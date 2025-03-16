# Proper Windows Reinstallation Guide <a href="https://ko-fi.com/byeoon">![Buy](https://img.shields.io/badge/Buy%20me%20a%20coffee!-byeoon-blue)</a>
**This guide is still being updated! Please be patient.**

### Intro
The correct way to reinstall Windows. This guide helps power users reconfigure a fresh system to squeeze out as much performance and user safety as possible. This is a guide made for Windows 11, but most parts are backwards comaptible. I personally do not use modded installations as they will always have random side effects such as not being able to use certain game launchers, core features being missing, and other things too. You can get the same, if not better performance just from following this guide. There was also [a video made by Eric Parker](https://www.youtube.com/watch?v=nyMHBKlNk9c&pp=ygUVZXJpYyBwYXJrZXIgbW9kZGVkIG9z) which talks about this more in detail.

### Index
Here is a short outline of the things that will be covered in this guide. It is recommended to read EVERYTHING though!
- 1. Pre-Installation
  - World Mode
  - LTSC Edition
- 2. Installation / OOBE
    - Bypass Microsoft Account Requirements
- 3. Post-OOBE
   - Tools to run
   - Optional Software for QoL
   - Mod your apps
 

## Pre-Installation
Before installing Windows (10/11) while you are still in the media creation tool for the least amount of bloatware **SET YOUR REGION TO American (World)**. I cannot stress this enough because it will remove so much initial bloat. This removes any 3rd party applications that Windows tries to install on boot (For example, candy crush, tiktok, solitaire) and leave your computer an almost blank slate. Some services like the Microsoft Store have been reported to be broken. If you don't care about that you can continue using World. If you do care, read the section below on installing the LTSC version of Windows.

### Installing Enterprise LTSC
To save you from all the hassle of putting in personal information, I will link the direct download for [Windows 11 LTSC here](https://drive.massgrave.dev/en-us_windows_11_iot_enterprise_ltsc_2024_x64_dvd_f6b14814.iso) and the [Windows 10 version here](https://drive.massgrave.dev/en-us_windows_10_iot_enterprise_ltsc_2021_x64_dvd_257ad90f.iso). The setup should be mostly similar but there will be even less bloat installed by default.

## Installation / OOBE
Of course, before installing, make sure to backup all your files on an external drive. Also, install Windows onto an NVME for the best performance. I use [this NVME](https://sabrent.com/products/sb-rocket-nvme4-1tb) but to be honest it's up to personal preference. <sub>This NVME in particular went on sale on Amazon for $50, so try to find deals like that.</sub>

If you followed the first part properly, you will see this when booting into the OOBE. The error message should say OOBEREGION. ![OOBEREGION](https://github.com/user-attachments/assets/540035b5-ae64-4644-b8cb-650da28e7840)

This means you set the region to **American (World)** and the bloat will not be installed! Great! You are already closer to a better Windows.

### LTSC Installation


### Local Account Setup
In recent Windows updates, they try to push you to have a permanently online account. They intentionally lock you out of making a local one during the initial setup but some smart people have figured out ways around this. Currently, the easiest way as of Windows 11 24H2 is to run a command in the internal developer console. **Press <kbd>CTRL</kbd> + <kbd>SHIFT</kbd> + <kbd>J</kbd> to open the developer console**. Once this is open, run `WinJS.Application.restart("ms-chx://LOCALONLY")`. You will now get pop up for creating a local account, enter your desired username and password and proceed with the setup like normal. 

Make sure to turn off all of the boxes for Microsoft to collect your data, or make them as optional and minimal as possible. Don't worry though, as once we reach the desktop we can completely get rid of telemetry. Once all of that is done, you should finally see your desktop!

## Post-OOBE
There are a few tools and commands that you should run and install first. This part is where everyone might forget to do or get stuck on.

