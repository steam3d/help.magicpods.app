# Infinite search

Sometimes when connecting AirPods, MagicPods may try to connect (or search for) headphones in endlessly. Even if the headphones are connected successfully and you are listening to music through them.
It looks like:

![](media/InfiniteSearch.gif)

For unknown reason Windows do not allow working with bluetooth and reboot doesn't help.

### Solution 1

Check some settings in The Windows

1. Close the MagicPods. Right click on MagicPods tray icon «Exit» or in MagicPods window click «Close MagicPods»
2. Open the Windows settings (Win+i)
3. Go to -> `Privacy` -> `Radios`. Turn off all switches and turn on again
4. Go to -> `Privacy` -> `Other Devices`. Turn off all switches and turn on again
5. Open the MagicPods and try to connect AirPods

![](media/InfiniteSearchWindowsSettings.gif)


### Solution 2

1. Close the MagicPods. Right click on MagicPods tray icon `Exit` or in MagicPods window click `Close MagicPods`
2. Update a Bluetooth driver to the latest version from manufacturer site. (Note: Windows update center may has not latest bluetooth driver)
3. Open the MagicPods and try to connect AirPods

If steps from above did not help, try to install the older Bluetooth driver instead the latest one.

### Solution 3

1. Close the MagicPods
2. Open `Task Manager` and terminate `MagicPodsService.exe` and `MagicPodsUI.exe` if they still work
3. Uninstall the MagicPods
4. `Important!` Reboot your PC
5. Install MagicPods

Usefully steeps above must help. if the problem still persists or you know a new solution, [create new issue.](report-issue.md)