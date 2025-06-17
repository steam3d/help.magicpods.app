# MagicAAP (Community) driver

!!! warning
    Requires MagicPods version 2.0.72.0 and above. Please don’t forget to create a system restore point.

The MagicAAP (Community) driver is the same version as [MagicAAP (Official)](fun-magicaap.md), but it was signed using a workaround by a member of our [community](https://discord.com/invite/UyY4PY768V).

As a downside, Windows Defender may flag the driver as potentially unwanted software, and some game anti-cheat systems might detect it.

You can read more about the discussion [here](https://discord.com/channels/1083322534675632188/1083322534675632191/1372238889988653108) and [here](https://discord.com/channels/1083322534675632188/1372235563163320330/1372235563163320330).

## Installation

To download and install the MagicAAP (Community) driver, follow the instructions below.

[Download](https://magicpods.app/utils/magicaap_community.zip){ .md-button .md-button--primary target=_blank}

```
SHA256          D971A287765D8076F2A84547EDCD34D6D6CDE4EF3C3C7A82DA6E28751C5A644F
```

### Automatic installation

1. Turn off Windows Defender:
    1. Open `Windows Security`
    2. Go to `Virus & threat protection`
    3. Click `Manage settings`
    4. Turn off `Real-time protection`
2. Double-click the file `install.bat`.
3. Wait — the driver will install automatically.
4. Turn Windows Defender back on.

### Manual installation

1. Turn off Windows Defender:
    1. Open `Windows Security`
    2. Go to `Virus & threat protection`
    3. Click `Manage settings`
    4. Turn off `Real-time protection`
2. Close the `MagicPods` application if it is running.
3. Change your computer's date:
    1. Click the clock in the bottom-right corner.
    2. Select `Date and time settings`.
    3. Turn off `Set time automatically`.
    4. Set the date to: **June 1, 2013**.
4. Find the file named MagicAAP.inf.
5. Right-click on it.
6. Choose `Install` from the context menu.
7. Confirm the installation if prompted.
8. Open `C:\Windows\System32\DriverStore\FileRepository`
9. Find a folder starting with `magicaap`
10. Add this folder to the Defender exclusions list.
11. Turn Windows Defender back on.

### Getting Started

> After installing the driver, you will find MagicAAP devices in the Bluetooth section of Device Manager.

You're ready to go. Launch MagicPods and connect your AirPods. Expand the settings for the AirPods you want, and you'll see the familiar iPhone-like settings.

## Uninstalling

To uninstall the MagicAAP (Community) driver, please refer to the uninstallation instructions below.

### Automatic uninstalling

1. Double-click the file `uninstall.bat`.
2. The driver will be removed automatically.


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
Signer Name:        Shenzhen yundian Technology Co., Ltd
```
5. Remember the value from `Published Name` (e.g., oem4.inf)
    * PAY CLOSE ATTENTION — IF YOU CHOOSE THE WRONG "PUBLISHED NAME", YOU MIGHT DELETE ANOTHER DRIVER
6. Enter the command below and press Enter to delete the driver (Replace oem4.inf with the actual value you found.):
```
pnputil /delete-driver oem4.inf /uninstall
```
   
7. Remove the `magicaap` folder from Defender exclusions.