# Proper Windows Reinstallation Guide <a href="https://ko-fi.com/byeoon">![Buy](https://img.shields.io/badge/Buy%20me%20a%20coffee!-byeoon-blue)</a>
**This guide is still being updated! Please be patient.** (Also thank you @deepytux for helping me with some sections!)

## Intro
This guide helps power users reconfigure a fresh system to squeeze out as much performance and user safety as possible. This is a guide made for Windows 11, but most parts are backwards comaptible. I personally do not use modded installations as they will always have random side effects such as not being able to use certain game launchers, core features being missing, and other things too. You can get the same, if not better performance just from following this guide. There was also [a video made by Eric Parker](https://www.youtube.com/watch?v=nyMHBKlNk9c&pp=ygUVZXJpYyBwYXJrZXIgbW9kZGVkIG9z) which talks about this more in detail.

### Index
Here is a short outline of the things that will be covered in this guide. It is recommended to read EVERYTHING!
- 1. Pre-Installation
  - World Region
  - LTSC Edition
- 2. Installation / OOBE
    - Bypass Microsoft Account Requirements
    - Force Local Account
- 3. Post-OOBE
   - Tools to run
   - Optional QoL Software
   - Mod your apps
     - Discord
     - Spotify
 

## Pre-Installation
Before installing Windows (10/11) while you are still in the media creation tool for the least amount of bloatware **SET YOUR REGION TO American (World)**. I cannot stress this enough because it will remove so much initial bloat. This removes any 3rd party applications that Windows tries to install on boot (For example, candy crush, tiktok, solitare) and leave your computer as an almost blank slate. Some services like the Microsoft Store have been reported to be broken on some installations of World. I have not had this issue occurr for me and if you don't care about that you can continue using World. If you care, read the section below on installing the Enterprise LTSC version of Windows as it is another good alternative.

If you really want to prepare, use [Ninite](https://ninite.com/) to get a complete auto installer of apps once when you are at the desktop environment. For the burning tool you can just use the media creation tool or [Rufus](https://rufus.ie/en/) if you are installing via an ISO.

### Installing Enterprise LTSC
The direct downloads for [Windows 11 LTSC are here](https://drive.massgrave.dev/en-us_windows_11_iot_enterprise_ltsc_2024_x64_dvd_f6b14814.iso) and the [Windows 10 version here](https://drive.massgrave.dev/en-us_windows_10_iot_enterprise_ltsc_2021_x64_dvd_257ad90f.iso). The OOBE setup should be practically the same, except the thing that makes LTSC better is that it **removes even more bloat than World**! LTSC gives you security updates for longer than regular Windows because you dont get any feature updates. For Windows 11 LTSC, it removes all TPM and secure boot requirements. It also doesn't have any Windows Store / UWP apps, and its mostly tailored for devices that require a reliable version of Windows. The only things that are left on the device are internal components like Notepad, CMD, and accessibility tools.

## Installation / OOBE
Of course, before installing, make sure to backup all your files on an external drive. It is reccomended to install Windows onto an NVME for the best performance. I use [this NVME](https://sabrent.com/products/sb-rocket-nvme4-1tb) but it's up to personal preference. <sub>This NVME in particular went on sale on Amazon for $49, so try to find deals like that.</sub>

If you followed the first part properly, you will see this when booting into the OOBE. The error message should say OOBEREGION. 

![OOBEREGION](https://github.com/user-attachments/assets/540035b5-ae64-4644-b8cb-650da28e7840)

This means you set the region to **American (World)** and the bloat will not be installed! Great! You are already closer to a fresher Windows.

### Local Account Setup
In recent Windows feature updates, they forcibly push you to have an online account. They intentionally lock you out of making a local one during the initial setup but some smart people have figured out ways around this. Currently, the easiest way as of Windows 11 24H2 is to run a bypass command in the developer console. **Press <kbd>CTRL</kbd> + <kbd>SHIFT</kbd> + <kbd>J</kbd> to open the developer console**. Once this is open, run `WinJS.Application.restart("ms-chx://LOCALONLY")`. You will now skip to the pop up for creating a local account, enter your desired username and password and proceed with the setup like normal. 

Make sure to turn off all of the boxes for Microsoft to collect your data, or make them as optional and minimal as possible. Don't worry though, as once we reach the desktop we can completely get rid of telemetry. Once all of that is done, you should finally see your desktop!

## Post-OOBE
There are a few tools and commands that you should run and install first. This part is where everyone might forget to do or get stuck on. The first thing that I made sure to download was [O&O ShutUp 10++](https://www.oo-software.com/en/shutup10), [Windows10Debloater](https://github.com/Sycnex/Windows10Debloater)/[Windows11Debloater](https://github.com/Raphire/Win11Debloat), [Remove MS Edge](https://github.com/ShadowWhisperer/Remove-MS-Edge), [Microsoft Activation Scripts](https://massgrave.dev/) (optional), and [Chris Titus Winutils](https://github.com/ChrisTitusTech/winutil). All of these play a crucial role in fine tuning your new Windows experience. If you want to tweak these yourself, skip to the next category. If you want to use my optimized configuration, the designated files will be put in the repository.

### Optional Quality of Life Software
There are some other tools that may help you adjust Windows to how you like it. [Winaero Tweaker](https://winaero.com)




