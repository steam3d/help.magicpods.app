# MagicAAP (Community) driver

!!! info
    Requires MagicPods version 2.0.72.0 and above. Please don’t forget to create a system restore point.

The MagicAAP (Community) driver is the same version as [MagicAAP (Official)](fun-magicaap.md), but it was signed using a workaround by a member of our [community](https://discord.com/invite/UyY4PY768V).

As a downside, Windows Defender may flag the driver as potentially unwanted software, and some game anti-cheat systems might detect it.

You can read more about the discussion [here](https://discord.com/channels/1083322534675632188/1445078913767444511).


## Quick installation

Run the command in PowerShell:

```
irm "https://magicpods.app/utils/magicaap-community-v1.ps1" | iex
```

<video controls style="max-width: 100%; height: auto;">
  <source src="/media/magicaap-community-install.mp4" type="video/mp4">
</video>

You're ready to go. Launch MagicPods and connect your AirPods. Expand the settings for the AirPods you want, and you'll see the familiar iPhone-like settings.

## Installation

To install the MagicAAP (Community) driver, please refer to the installation instructions below.

### Automatic installation

1. Turn off Windows Defender:
    1. Open `Windows Security`
    2. Go to `Virus & threat protection`
    3. Click `Manage settings`
    4. Turn off `Real-time protection`
2. Open PowerShell:
    1. Press Win, type `PowerShell`, and open it.
3. Run a command:
```
irm "https://magicpods.app/utils/magicaap-community-v1.ps1" | iex
```
4. When the "Command Prompt" window opens:
    1. Type 1 and press Enter.
5. Wait — the driver will install automatically.
6. Done. Type 3 and press Enter to exit and close `PowerShell`.

### Manual installation

[Download](https://magicpods.app/utils/magicaap_community_v1.zip){ .md-button .md-button--primary target=_blank}

```
SHA256          607637CACB7B4CEA163CFE5B4DAADECF7CCBDE04D0FFF49A27BEBC7012B138C8
```

1. Turn off Windows Defender:
    1. Open `Windows Security`
    2. Go to `Virus & threat protection`
    3. Click `Manage settings`
    4. Turn off `Real-time protection`
2. Close the `MagicPods` application if it is running.
3. Find the file named AddCert.reg.
4. Double click on it. The certificate JemmyLoveJenny EV Root CA will be imported.
5. Find the file named MagicAAP.inf.
7. Right-click on it.
7. Choose `Install` from the context menu.
8. Confirm the installation if prompted.
9. Open `C:\Windows\System32\DriverStore\FileRepository`
10. Find a folder starting with `magicaap`
11. Add this folder to the Defender exclusions list.
12. Turn Windows Defender back on.

## Uninstalling

To uninstall the MagicAAP (Community) driver, please refer to the uninstallation instructions below.

### Automatic uninstalling

1. Open PowerShell:
    1. Press Win, type `PowerShell`, and open it.
2. Run a command:
```
irm "https://magicpods.app/utils/magicaap-community-v1.ps1" | iex
```
3. When the `Command Prompt` window opens:
    1. Type 2 and press Enter.
4. The driver will be removed automatically.
5. Done. Type 3 and press Enter to exit and close `PowerShell`.


### Manual uninstalling

1. Close the MagicPods application if it is running.
2. Open PowerShell as Administrator:
    1. Click the Start button.
    2. Type PowerShell.
    3. Right-click on the result.
    4. Select `Run as administrator`.
3. Enter the following command and press Enter:
```
pnputil /enum-drivers
```
4. Look for a block similar to this:
```
Published Name:     oem4.inf
Original Name:      magicaap.inf
Provider Name:      IP Maslov Alexander Yuryevich
Class Name:         Bluetooth
Class GUID:         {e0cbf06c-cd8b-4647-bb8a-263b43f0f974}
Driver Version:     06/06/2024 0.0.0.1
Signer Name:        Hubei Dadi Network Technology Co., Ltd.
```
5. Remember the value from `Published Name` (e.g., oem4.inf)
    * PAY CLOSE ATTENTION — IF YOU CHOOSE THE WRONG "PUBLISHED NAME", YOU MIGHT DELETE ANOTHER DRIVER
6. Enter the command below and press Enter to delete the driver (Replace oem4.inf with the actual value you found.):
```
pnputil /delete-driver oem4.inf /uninstall
```
7. Remove the `magicaap` folder from Defender exclusions.