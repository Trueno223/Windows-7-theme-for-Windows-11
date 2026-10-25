# Windows 7 theme for Windows 11
This theme uses third-party apps and built-in Windows features, so it may keep working on future versions, but updates can still break it.
This theme should be reversible as it does not replace or permanently modify any system files.[^1]
[^1]: Windhawk and Winaero Tweaker inject into running processes and change registry settings rather than replacing system files. Both can revert to default settings.

<details>
<summary>Expand for screenshots</summary>

<br>

<img width="1919" height="1034" alt="Windows programs with Windows 7 theming" src="https://github.com/user-attachments/assets/c8765e19-c2ed-44be-8187-e21945513a22" />

<img width="433" height="562" alt="Windows start menu with Windows 7 theming" src="https://github.com/user-attachments/assets/f040bd53-9273-49d5-a30e-f8abbc95a29c" />

(May differ from your results because I had different personalization settings!)

</details>

# Table of Contents
* [Prerequisites](#what-youll-need)
* [Installation](#installation-and-settings)
  - [Aero10.1](#aero101)
  - [StartAllBack](#startallback)
  - [OpenGlass](#openglass)
  - [Windhawk](#windhawk)
  - [Winaero Tweaker](#winaero-tweaker)
  - [Mouse Theme](#mouse-theme)
  - [Sound Theme](#sound-theme)
* [Uninstall](#uninstall)
* [Credits](#credits)
* [Final notes](#final-notes)

# What you'll need:
- [Aero10.1](<https://github.com/vaporvance/aero10>)
- [StartAllBack](https://www.startallback.com/) (Paid, free trial)
- [OpenGlass](<https://github.com/ALTaleX531/OpenGlass>)
- [Windhawk](https://windhawk.net/)
- [Winaero Tweaker](https://winaerotweaker.com/)

# Installation and settings
> [!WARNING]
> Make sure to create a [System Restore Point](https://www.minitool.com/news/create-a-system-restore-point-windows-11.html) in case something breaks!

## Aero10.1
Follow the [installation steps](https://github.com/vaporvance/aero10#installation) from Aero10.1 GitHub page and apply the theme, then proceed to the next steps.

## StartAllBack
After installing this program you can select the "Remastered 7" preset in the Welcome screen to automatically apply the Windows 7 taskbar and start menu theme. Further modification is your preference.
If you wish to recreate the Windows 7 File Explorer with StartAllBack do the following:
1. Navigate to the "Explorer" tab in StartAllBack Configuration
2. Enable "Win7 Command Bar"
3. Enable "Mica effect on top"
4. Enable "Classic context menus"

## OpenGlass
After installing OpenGlass run the "Configure OpenGlass" shortcut on your desktop and apply the following settings:

In Appearance tab:
- Blur amount: 4
- Glass geometry radius: Windows 7 style
- Caption buttons style: Windows 7 style
- Disable modern borders: :white_check_mark:
- Text glow mode: Use theme atlas
- Override accent: :white_check_mark:

<details>
<summary>Context menus unreadable? Expand this for the fix</summary>

<br>

If "Override accent" makes context menus unreadable, disable it and enable transparency in StartAllBack instead:

1. Open StartAllBack configuration and go to the "Advanced" tab
2. Enable "Use custom start menu coloring", set the look to Blur (the :droplet: icon), and set opacity to 0%
3. Enable "Use custom taskbar coloring" and repeat the same steps

[This issue](https://github.com/ALTaleX531/OpenGlass/issues/376) might be resolved in future versions of OpenGlass.

</details>

In Glass colors tab:
- Glass type: Windows 7 aero
- Color presets: Sky (or your preference)
- Enable transparency: :white_check_mark:

## Windhawk
After installing Windhawk navigate to the Explore tab and search and install the following extensions:
1. Resource Redirect
2. Legacy File Copy
3. Force thick frames

After installing the extensions navigate back to the Home tab and click on the Details button of Resource Redirect and go to settings:
- Select the icon theme "Pane7 (by ImSwordQueen)"
- Enable "Disable folder thumbnails" to avoid some visual bugs.

## Winaero Tweaker
After installing Winaero Tweaker open it and do the following:
1. Search for "shortcut arrow" and enable "Classic arrow"
2. Search for "windows photo viewer" and press the "Activate Windows Photo Viewer" button
3. (optional) Search for "startup sound", enable it and replace the sound with the Windows 7 one. (You can get the sound [here](https://www.winhistory.de/more/winstart/winstart_en.htm))

## Mouse theme
You can get the Windows 7 mouse cursor theme [here](https://www.rw-designer.com/cursor-set/windows-7-classic-edition) and to install it do the following:
1. Navigate to `C:\Windows\Cursors` and make a new folder called "Windows 7 Cursors", or whatever name you prefer, and extract the cursors into that folder (requires admin rights)
2. Type "main.cpl" in the start menu and hit enter
3. In the newly opened window go to "Pointers" tab
4. Select each image from `C:\Windows\Cursors\Windows 7 Cursors` and apply it to each cursor, the icon names are roughly the same as the cursor function name so it shouldn't be hard.
5. Check "Enable pointer shadow" for a more Windows 7-like look
6. Optional but you can save your mouse theme

## Sound theme
You can get the Windows 7 sound theme [here](https://levithon.itch.io/windows-7-sound-pack-all-themes) and to install it do the following:
1. Navigate to `C:\Windows\Media` and extract the 'Windows 7 Sounds' folder here (requires admin rights)
2. Type "mmsys.cpl" in the start menu and hit enter
3. In the newly opened window go to "Sounds" tab
4. Apply the following sounds:
  - Windows
    - Asterisk - Windows Exclamation.wav
    - Calendar Reminder - Windows Exclamation.wav
    - Critical Battery Alarm - Windows Battery Critical.wav
    - Critical Stop - Windows Critical Stop.wav
    - Default Beep - Windows Ding.wav
    - Desktop Mail Notification - Speech On.wav
    - Device Connect  - Windows Hardware Insert.wav
    - Device Disconnect - Windows Hardware Remove.wav
    - Device Failed to Connect - Windows Hardware Fail.wav
    - Exclamation - Windows Exclamation.wav
    - Instant Message Notification - Windows Notify.wav
    - Low Battery Alarm - Windows Battery Low.wav
    - Message Nudge - Windows Notify.wav
    - Notification - Windows Notify.wav
    - Question - Windows Notify.wav
    - System Notification - Windows Notify.wav
    - (you might need to edit the registry for the following 3 to show up)
    - Windows Logoff - Windows Logoff Sound.wav[^2]
    - Windows Logon - Windows Logon Sound.wav[^2]
    - Windows User Account Control - Windows User Account Control.wav[^2]
  - File Explorer
    - Empty Recycle Bin - Windows Recycle.wav
    - Start Navigation - Windows Navigation Start.wav
[^2]: You might need to [edit the registry](https://thegeekpage.com/enable-logoff-and-logon-sounds/#Method_2_Using_Registry_Editor) for these to show up

5. Optional but you can save your sound theme.

# Uninstall
## Theme
Disable the Windows 7 theme from settings (select Windows (light) or Windows (dark) making sure it's not a Aero10.1 theme)
Navigate to 'C:\Windows\Resources\Themes' and delete the following:
- aero10p1 (folder)
- Aero10.1 Seven (Dark).theme
- Aero10.1 Seven.theme

## Apps
To uninstall the taskbar, start menu and window borders type "appwiz.cpl" in the start menu and uninstall:
- Winaero Tweaker (you might have to open Winaero Tweaker first and manually set everything back to default)
- OpenGlass
- Windhawk
- StartAllBack
- SecureUxTheme (or whatever method you used to allow custom themes)

## Cursors
To revert to the default mouse theme type "main.cpl" in the start menu and go to the "Pointers" tab and select the "Windows Default (system scheme)" scheme.
Navigate to `C:\Windows\Cursors` and delete "Windows 7 Cursors" (or whatever you called it)

## Sounds
To revert to the default sounds type "mmsys.cpl" in the start menu and go to the "Sounds" tab and select the "Windows Default" scheme.
Navigate to `C:\Windows\Media` and delete the 'Windows 7 Sounds' folder.

# Credits
This tutorial was inspired by LagLife on YouTube. Check out [their video](https://youtu.be/FqKw_KCIGK4) on transforming Windows 11 to Windows 7.

# Final notes
- This theme was tested on Windows version 26H2 26300.9711, future versions might break it!
- If you'd like to add, edit or remove something from this tutorial feel free to open an issue ticket (eg. free alternative to StartAllBack).
- StartAllBack and Windhawk can conflict with anti-cheat in some games! Disable these if you run into issues.
- Sadly this tutorial doesn't cover modifying tray icons or the context menu, if you find a way to do this open an issue ticket!
