## 2.0.39.0 (04-01-2023)

🎉 Meet 2023 with new update and new features. 
Introduce «Audio streaming» feature. Stream audio from your Bluetooth devices to your PC. The PC acts as a Bluetooth speaker. (Required Windows 10 19041)

New:

- Audio streaming feature
- Popup window when sound out changed

Updated:

- Changed logic of fast search. Now ear detection works much faster
- Headphone names in context menu sorted by its name now

The update is very complex and tested on Windows 10 18362, Windows 10 17763, and Windows 11.

## 2.0.38.0 (27-11-2022)

For some users, the headphone list was empty.

Fixed:

- VoiceOver was causing the headphones detection to crash when Windows does not have any installed voice
- Update live tile was causing the application to crash when Windows has trouble with notification service
- Accessing an audio device could cause the app to crash

Updated:

- Translations for most languages.

The update is very complex and tested on Windows 10 18362, Windows 10 17763, and Windows 11.

## 2.0.32.0 (29-11-2022)

The entire logic of the application has been completely rewritten, which made it possible to add the ability to connect and disconnect any Bluetooth headphones.

Added:

-   Support for some functions for any Bluetooth headphones
-   Change headphone image
-   Dynamic watching of available Bluetooth headphones in the system
-   Dynamic watching of available Bluetooth adapters in the system
-   Enable Bluetooth from the main application window
-   Updated tooltips for problems with Bluetooth adapters
-   Updated tray icons
-   Updated headphone icons in the context menu
-   «Ear detection» supports multiple connected headphones. (Detailed in help.magicpods.app)

Changed:

- Disabled some non-working AirPods Pro 2 features (detailed at help.magicpods.app/fun-capability)

Updated:

- Translations for most languages.

The update is very complex and tested on Windows 10 18362, Windows 10 17763, and Windows 11.

## 2.0.5.0 (27-09-2022)

- Added experimental support 🎧AirPods Pro 2.
- Added and updated languages
- Fixed issue when «Low audio latency» toggle does not work

## 2.0.4.0 (05-08-2022)

A small change under the hood, maybe some users will have a more stable connection with the headphones.

Fixed:

- Accent color was wrong when the user chooses the Light theme in app when the Windows theme was dark
- Fixed problem with exiting the app

Updated:

- Changed connection button style

Added languages:

- Czech (Czech Republic)
- Indonesian (Indonesia)
- Thai (Thailand)

## 2.0.3.0 (09-07-2022)

- Added Beats Studio Buds support
- Fixed ToggleSwitch in headphones settings
- Updated translations for some languages

## 2.0.2.0 (04-07-2022)

- Fixed issue when you open the app it crashes
- Updated translations

## 2.0.1.0 (01-07-2022)

- Fixed Auto-Pause issue
- Updated translations

## 2.0.0.0 (30-06-2022)

Meet MagicPods✨ 2.0

Completely redesigned look and feel to match the new Windows 11 look and feel. The interface logic has been rethought, making it more intuitive and especially convenient for users with multiple headphones.

Added new settings:

- Hotkey to connect and disconnect headphones
- Headphone low battery notification
- Auto-pause when headphones disconnected, or the screen is locked

UI updated:

- Added a card for each headphone, which contains all the available settings
- Added new animated battery icon
- Added tips how to pair headphones with a computer, Bluetooth is turned off, etc.
- Redrawn welcome animations
- Icons in the menu have been redrawn, now they are more detailed

Fixed:

- Bug where the option «Show AirPods charge on icon» was disabled, and when hovering over the icon in the tray, the battery charge was not displayed
- Bug when after turning off and on Bluetooth, pressing the connect button did not work
- Notification when Bluetooth module is not supported.
- Some texts could not be translated into another language
- Reduced memory consumption
- Significantly reduced the size of the application

## 1.0.84.0 (15-05-2022)

- Updated translations

## 1.0.83.0 (19-03-2022)

Added a new way to connect AirPods. It made connecting AirPods faster and added an AirPods disconnect feature.
The design of the pop-up menu by clicking on the icon in the notification area has been completely redesigned. It now matches the look and feel of Windows 10 and 11.

Fixed:

- Disabled Bluetooth audio services are no longer enabled after AirPods are connected.

## 1.0.81.0 (27-01-2022)

Added new headphones supports:

- Beats Fit Pro
- Beats Solo 3 (only battery)
- Beats Solo Pro (only battery)
- Beats Studio 3 (only battery)
- Beats X (only battery)
- Beats Flex (only battery)
- Power Beats 3 (only battery)

Fixed:

- AirPods Max ear detection 
- VoiceOver read text multiple times when user lock and unlock the screen

Updated translations.

## 1.0.80.0 (04-01-2022)
Introducing Mica - new Windows 11 material. For Windows 11 users the MagicPods will use Mica material instead of acrylic material.

What's new?

- The appearance has been updated, now it is more in line with Windows 11 style
- Manual switching of light and dark themes. Separately for the popup window and for the application itself.
- Multiple display support. The pop-up window will no longer flash, appear in the wrong position or outside the monitor when connecting external monitors. The tray icon will always be clear, even if you change the scaling in the system
- Improve popup performance and animation
- Switch language

Fixed:

- Flashing text when you open the MagicPods for the first time.
- Animation played too fast after hibernation

Add new languages:

- Danish
- Greek
- Serbian (Latin)
- Sinhala

Updated all language translations. Thanks to our community for the work done.

Do not forget to report problems in the support section.
If you have problems after update, try reinstalling the application and reboot PC.

## 1.0.79.0 (01-11-2021)

Say hello to your 🎧 AirPods 3 

- Updated languages
- Add supports AirPods 3

## 1.0.78.0 (16-09-2021)

⚠️ Warning MagicPods has changed the architecture of the application to better support Windows 11. If you have problems, please reinstall the application.

Meet Windows 11 support

- Updated user interface
- Updated logo
- Added tooltips

Fixed:

- An error that caused the application to crash when the user connects AirPods

## 1.0.75.0 (16-09-2021)

New:

- Smoothly decrease and increase the volume when the earbud is removed from your ear
- Now, after disconnect the AirPods, the audio players will be paused if they were playing sound
- Auto switch audio output no longer requires additional components to install

New languages:

- Vietnamese
- Updated other languages

Fixed:

- An error that caused the application to crash when the user turned off the Bluetooth
- An error that caused the application to crash when VoiceOver read notification
- An error where animation played incorrectly on monitors with high refresh rate
- An error that caused the application to crash when selecting some applications from the list VoiceOver apps
- An error in which the animation in the "Status" window blinked when fast search was enabled

## 1.0.74.0 (19-07-2021)

Fixed hide popup window when click outside. (Not works on some pc)

## 1.0.73.0 (17-07-2021)

The popup will now hide when you click outside of it.

- Added Romanian, Japanese and Polish languages
- Updated some languages

## 1.0.72.0 (30-06-2021)

- Added support Play / Pause for iTunes (Microsoft store)
- Added the ability connect the AirPods from tray menu
- Fixes bug when connecting AirPods with some disabled services caused the app to crash.
- Updated translations (Thx our community)

## 1.0.71.0 (22-05-2021)

Say hello to your AirPods Max 👋

New:

- Add supports AirPods Max
- Improved response from opening and closing AirPods case
- Updated translations in many languages
- Changed the hiding time of the pop-up window from 10 seconds to 30 seconds when clicking on the cross.

## 1.0.70.0 (23-04-2021)

This update brings new feature «VoiceOver notification». The built-in announcer will read out new notifications.
Don't worry, the MagicPods does not collect any data, everything is stored only on your computer.

- Added Swedish, Ukrainian, Italian
- Updated some languages
- Added new wiki

## 1.0.68.0 (18-03-2021)

This update will optimize the application.

- Reduce power consumption
- Reduce RAM consumption
- Fixed bug when video blink before start playing
- Bug fixes

## 1.0.66.0 (21-02-2021)

- Fixed crashed the app when after switch user
- Fixed crashed the app when the user has disabled some audio services
- Updated and supplemented translation of some languages
- Added Hungarian language

## 1.0.65.0 (02-02-2021)
- Fixed issue when some users have crashed the settings window.

## 1.0.63.0 (01-02-2021)
- Hot fix crash menu for Windows 10 build 18362 and down

## 1.0.61.0 (31-01-2021)

- Updated all languages. Thx our community for the help.
- Added connect icon. (Shows when the app is connecting headphones)
- MagicPods name returned to title bar
- Replace header name to title bar. (Especially useful in the small window where free space is important)
- Fixed issue when some Bluetooth data could crash the app
- Changed some default settings. (Applies only to new installation of the application)

## 1.0.60.0 (24-01-2021)

- Added tooltip for "Auto switch audio output".
- Updated Korean, English and Russian languages.

## 1.0.58.0 (11-01-2021)

The large update brings some new features:

- Auto switch audio output
- Animation position on screen
- New search status animation and icon for it
- Reduce RAM consumption
- Battery step changed from 0%, 10%, 20% ... to 5%, 15%, 25% ...
- Connect button color now uses windows accent color

Added languages:

- Dutch
- German

Note. Translation in some languages is incomplete.

## 1.0.55.0 (23-11-2020)

- Added Korean language 
- Updated translation of the «Connect» button
- Fixed a bug where the low battery notification sometimes displayed the wrong charge


## 1.0.43.0 (04-11-2020)

- Added Turkish language
- Bug fixes

## 1.0.42.0 (20-09-2020)

Introducing a new interface with Microsoft Fluent Design.

New features:

- You can now connect to your AirPods through pop-up window or automatically.
- Supports all media players with system media control (detailed information in the app).
- In addition, VLC, QQMusic, CloudMusic, KuGou are also supported.
- Auto play command when you connect to your AirPods.

Bug fixes:

- Sometimes other Apple device can crash the app.


## 1.0.37.0 (05-08-2020)

- Fixed grammar errors.
- Added languages:
- Chinese (Taiwan)
- French (France)
- Portuguese (Brazil) - partially translated

## 1.0.35.0 (26-07-2020)

- Added Chinese language

## 1.0.33.0 (22-07-2020)

- Added support PowerBeatsPro (beta).
- Added hover text on tray icon.
- Added digital battery information tray icon.
- Added Auto switch dark / light theme for tray icon.

Improved AirPods search.

- Fixed notification with error "Bluetooth low energy does not support". Now if you hide tray icon you will able to close the app.
- Fixed an error that caused to slow frame rate of animation. Now animation plays at 60fps
- Fixed an error that caused to moving the name of the headphones to the second line 
- Fixed an error that caused to trouble with play / pause. Now you can retranslate audio signal or listening your - microphone without blocking play / pause option.

Deleted legacy method of search AirPods. Let me know if you have trouble.

## 1.0.28.0 (14-06-2020)

You asked, I did! Now you can choose size of animation window. Also you can watch battery level on icon tray.

- Added Russian language.
- Fixed a bug when the charge icon on the right earphone was not displayed

## 1.0.25.0 (19-05-2020)

- Fixed a bug when the CPU was loaded at 100% if the Bluetooth is off
- improved performance to Splash screen animation
- Fixed flickering of Splash screen animation
- Improved UI. The welcome page has been deleted and now it’s not confusing
- The application no longer crashes when there are no audio devices in the system

## 1.0.22.0 (08-05-2020)

- [Fixed steam3d/MagicPods-Windows#5](https://github.com/steam3d/MagicPods-Windows/issues/5)
- added Fast search settings

## 1.0.21.0 (06-05-2020)

- Play / Pause for couple apps. It doesn't work very well, but it works :)
- New status page. Connect to AirPods and open the app.
- Hide tray icon option.
- Low audio latency. Useful for audio and video editors.
- Fixed settings. Now app will not restore settings after update.
- New video player. Now the video should not fade or turn to black

Fixed an issue where the charge was displayed incorrectly

## 1.0.17.0 (26-03-2020)

- Fixed AirPods Pro crush.
- Fixed DeviceVideos IDs

## 1.0.16.0 (26-03-2020)

- Fixed Broken Animation screen for AirPods Pro

## 1.0.15.0 (25-03-2020)
- Added AirPods Pro support
- Search device by model ID
- Detect connect of bluetooth device by system event
- Software render for video

## 1.0.12.0 (05-03-2020)

First release.

- Animation
- Battery
- Dark and Light theme
- Notification
- Live tile