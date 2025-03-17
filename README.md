# Proper Windows Reinstallation Guide <a href='https://ko-fi.com/O5O6VWWOH' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi5.png?v=6' alt='Buy Me a Coffee at ko-fi.com' /></a>
**This guide is still being updated! Please be patient. Last updated 3/17/25** (Also thank you @deepytux for helping me with some sections!)

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
There are two different ways to optimally install Windows, it depends on personal preference.

### English (World)
Before installing Windows (10/11) while you are still in the media creation tool **SET YOUR REGION TO American (World)**. If you do not see the option in the media tool, you will have to do that in the setup itself (image below).  This removes any 3rd party applications and bloat that Windows tries to install on start such as Candy Crush, TikTok, and Solitare. Some services like the Microsoft Store and core functions have been reported to be broken on some installations of World. I have not had any issues occurr for me and if you don't care about those potential risks you can continue using World. If you care, read the `Enterprise LTSC` section. It is a great alternative to World, if not better in some cases. 

<img src="https://github.com/user-attachments/assets/13342b8b-4fa7-439f-aa45-d8b067c760b8" height="480px" width="480px">

### Enterprise LTSC
The direct downloads for [Windows 11 LTSC are here](https://drive.massgrave.dev/en-us_windows_11_iot_enterprise_ltsc_2024_x64_dvd_f6b14814.iso) and the [Windows 10 version here](https://drive.massgrave.dev/en-us_windows_10_iot_enterprise_ltsc_2021_x64_dvd_257ad90f.iso). Since these are ISO files when downloaded, you will need to burn it to a flash drive. I recommend using [Rufus](https://rufus.com) to do that.

## OOBE
Of course, before installing, make sure to backup all your files on an external drive. It is reccomended to install Windows onto an NVME for the best performance. I use [this NVME](https://sabrent.com/products/sb-rocket-nvme4-1tb) but it's up to personal preference. <sub>This NVME in particular went on sale on Amazon for $49, so try to find deals like that.</sub>

If you followed the first part properly, you will see this when booting into the OOBE. The error message should say OOBEREGION. 

![OOBEREGION](https://github.com/user-attachments/assets/540035b5-ae64-4644-b8cb-650da28e7840)

This means you set the region to **American (World)** and the bloat will not be installed! Great! You are already closer to a fresher Windows.

### Local Account Setup
In recent Windows feature updates, they forcibly push you to have an online account. They intentionally lock you out of making a local one during the initial setup but some smart people have figured out ways around this. Currently, the easiest way as of Windows 11 24H2 is to run a bypass command in the developer console. **Press <kbd>CTRL</kbd> + <kbd>SHIFT</kbd> + <kbd>J</kbd> to open the developer console**. Once this is open, run `WinJS.Application.restart("ms-chx://LOCALONLY")`. You will now skip to the pop up for creating a local account, enter your desired username and password and proceed with the setup like normal. 

Make sure to turn off all of the boxes for Microsoft to collect your data, or make them as optional and minimal as possible. Don't worry though, as once we reach the desktop we can completely get rid of telemetry. Once all of that is done, you should finally see your desktop!

## Post-OOBE
There are a few tools and commands that you should run and install first. This part is where everyone might forget to do or get stuck on. The first thing that I made sure to download was [O&O ShutUp 10++](https://www.oo-software.com/en/shutup10), [Windows10Debloater](https://github.com/Sycnex/Windows10Debloater)/[Windows11Debloater](https://github.com/Raphire/Win11Debloat), [Remove MS Edge](https://github.com/ShadowWhisperer/Remove-MS-Edge), [Microsoft Activation Scripts](https://massgrave.dev/) (optional), and [Chris Titus Winutils](https://github.com/ChrisTitusTech/winutil). All of these play a crucial role in fine tuning your new Windows experience. If you want to tweak these yourself, skip to the next category.

### O&O ShutUp 10++
If you want to use my configuration file, it's in the repository and [you can download it here](https://github.com/byeoon/Proper-Windows-Reinstall/blob/master/Byeoon%20OOSU10%20Config.cfg). To apply the changes, go to `File > Import Settings` and then select the config file you just downloaded.

### Optional Quality of Life Software
There are some other tools that may help you adjust Windows to your liking. [Winaero Tweaker](https://winaero.com) is one that I personally use on every reinstall because it has a bunch of customizable features 




