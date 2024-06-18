# MagicAAP driver

!!! warning
    Only install the MagicAAP driver if you are an advanced user and are prepared to reinstall Windows if problems occur. Requires MagicPods version 2.0.72.0 and above.
    
MagicAAP is a Bluetooth profile driver that allows you to add near-full support for all AirPods and some Beats headphones.

![](/media/MagicAAP-Driver-Sample.png)


## Installation

The MagicAAP driver is not yet digitally signed, so you will need to switch Windows into test mode to install it. A message will appear in the bottom right corner of the screen indicating that Windows is in test mode.

### 0. Create a restore point

1. Press `Start` and type `Create a restore point` in the search box
2. In the search results, select `Create a restore point`
3. In the window that opens, click `Create`
![](/media/MagicAAP-Restore-Point.png)
3. Type the title and press `Create`
![](/media/MagicAAP-Restore-Point-Create.png)

If there are any problems, you can use this restore point to restore Windows. If you use BitLocker, you will also need a recovery code.


### 1. Copy the BitLocker recovery key

If you are using BitLocker, BitLocker will detect the change in system settings and request a recovery key. You will need to enter the key twice during the installation process.

| Icon                                   | Description   |
| -------------------------------------- | ------------- |
| ![](/media/MagicAAP-Bitlocker-Off.png) | BitLocker off |
| ![](/media/MagicAAP-Bitlocker-On.png)  | BitLocker on  |

1. Open my computer. Right-click the drive with the lock icon and select `Manage BitLocker` from the context menu  
![](/media/MagicAAP-Bitlocker-Manage.png)
2. In the window that opens, click `Back up your recovery key` and follow the instructions  
![](/media/MagicAAP-Bitlocker-Recovery-Key.png)
3. Repeat the process for each drive that uses encryption

Keep the recovery codes in your phone, notebook, or on another computer because you will need to enter the recovery code before Windows starts.

> I recommend using the Google query [BitLocker recovery key](https://www.google.com/search?q=BitLocker+recovery+key) for more detailed instructions.

### 2. Disable Secure Boot

1. Enter your computer's BIOS. Normally, when you turn on your computer, you will need to press one of the F1, F2, F12 or Esc keys to enter the BIOS
2. Find the `Secure Boot` option in the BIOS settings and disable it  
![](/media/MagicAAP-Secure-Boot-Disabled.png)
3. Save your changes and restart your computer
4. If you are using BitLocker, enter the `Recovery key` while the computer is booting  
![](/media/MagicAAP-Bitlocker-Recovery.png)

> I recommend using the Google query [Disable Secure Boot](https://www.google.com/search?q=Disable+Secure+Boot) for more detailed instructions.

### 3. Switch Windows to test mode

1. Right-click on the Windows icon
2. From the context menu, select `Terminal (Admin)` or `PowerShell (Admin)`  
![](/media/MagicAAP-Terminal-Admin.png)
3. Enter command:
```
bcdedit /set testsigning ON
```
![](/media/MagicAAP-Testsigning-On.png)
4. Restart the computer  
5. If you are using BitLocker, enter the `Recovery key` while the computer is booting  
![](/media/MagicAAP-Bitlocker-Recovery.png)

### 4. Install the MagicAAP driver

Optionally you can check the integrity of the [magicaap.zip](https://magicpods.app/utils/magicaap.zip)


```
SHA256          E16A8F1C6052432A388D33FDD4AC6D4F3CA909CF4C3DD37A152DB0E9342B66C2
```

#### Automatic installation

1. [Download MagicAAP driver](https://magicpods.app/utils/magicaap.zip)  
2. Unzip the driver archive and navigate to the driver folder
3. Right-click on `MagicAAP.inf` and select `Install` in the context menu  
![](/media/MagicAAP-Driver-Install-Auto.png)
4. Confirm the installation of an unsigned driver  
![](/media/MagicAAP-Driver-Install-Warning.png)

#### Manual installation

1. [Download MagicAAP driver](https://magicpods.app/utils/magicaap.zip)
2. Unzip the driver archive
3. Press `Start` and type `Device Manager` in the search box
4. In the search results, select `Device Manager`
5. In `Device Manager`, find `AAP Server` in the `Other devices` section
6. Right-click on it and select `Update driver` from the context menu  
![](/media/MagicAAP-Manual-Update-Driver.png)
7. In the window that opens, click on `Browse my computer for drivers`, then specify the path to the driver folder  
![](/media/MagicAAP-Manual-Update-Driver-Install.png)
8. Click `Next`, the driver will be installed
9. Repeat steps 5-8 for each `AAP Server` device

You're ready to go. Launch MagicPods and connect your AirPods. Expand the settings for the AirPods you want, and you'll see the familiar iPhone-like settings.

## Uninstalling

To uninstall the driver and return Windows to normal mode, repeat the installation steps in reverse order.

### 1. Copy the BitLocker recovery key

If you are using BitLocker, BitLocker will detect the change in system settings and request a recovery key. You will need to enter the key twice during the uninstalling process.

| Icon                                   | Description   |
| -------------------------------------- | ------------- |
| ![](/media/MagicAAP-Bitlocker-Off.png) | BitLocker off |
| ![](/media/MagicAAP-Bitlocker-On.png)  | BitLocker on  |

1. Open my computer. Right-click the drive with the lock icon and select `Manage BitLocker` from the context menu  
![](/media/MagicAAP-Bitlocker-Manage.png)
2. In the window that opens, click `Back up your recovery key` and follow the instructions  
![](/media/MagicAAP-Bitlocker-Recovery-Key.png)
3. Repeat the process for each drive that uses encryption

Keep the recovery codes in your phone, notebook, or on another computer because you will need to enter the recovery code before Windows starts.

> I recommend using the Google query [BitLocker recovery key](https://www.google.com/search?q=BitLocker+recovery+key) for more detailed instructions.


### 2. Uninstalling the MagicAAP driver

1. Press `Start` and type `Device Manager` in the search box
2. In the search results, select `Device Manager`
3. In `Device Manager`, find `MagicAAP` in the `Bluetooth` section
4. Right click on it and select `Uninstall driver` in the context menu  
![](/media/MagicAAP-Manual-Uninstall-Driver.png)
5. Check `Attempt to remove the driver for this device.` and click `Uninstall`  
![](/media/MagicAAP-Manual-Uninstall-Driver-Uninstall.png)
6. Repeat steps 3-5 for each `AAP Server` device

### 3. Switch Windows to normal mode

1. Right-click on the Windows icon
2. From the context menu, select `Terminal (Admin)` or `PowerShell (Admin)`  
![](/media/MagicAAP-Terminal-Admin.png)
3. Enter command:
```
bcdedit /set testsigning OFF
```
![](/media/MagicAAP-Testsigning-Off.png)
4. Restart the computer  
5. If you are using BitLocker, enter the `Recovery key` while the computer is booting  
![](/media/MagicAAP-Bitlocker-Recovery.png)

### 4. Enable Secure Boot

1. Enter your computer's BIOS. Normally, when you turn on your computer, you will need to press one of the F1, F2, F12 or Esc keys to enter the BIOS
2. Find the `Secure Boot` option in the BIOS settings and enable it  
![](/media/MagicAAP-Secure-Boot-Enabled.png)
3. Save changes and restart your computer
4. If you are using BitLocker, enter the `Recovery key` while the computer is booting  
![](/media/MagicAAP-Bitlocker-Recovery.png)  

All done. Windows will now run normally and the message in the bottom right-hand corner of the desktop will no longer appear.