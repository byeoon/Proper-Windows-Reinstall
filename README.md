# Proper Windows Reinstallation Guide <a href='https://ko-fi.com/O5O6VWWOH' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi5.png?v=6' alt='Buy Me a Coffee at ko-fi.com' /></a>
**This guide is still being updated! Please be patient. It was last updated on 6/10/25**

## Intro
This guide helps power users reconfigure a fresh system to squeeze out as much performance and user safety as possible. This is a guide made for Windows 11 but most parts are backwards comaptible. I personally do not use modded installations as they will always have random side effects such as not being able to use certain game launchers, core features being missing, and other things too. You can get the same, if not better performance just from following this guide. There was also [a video made by Eric Parker](https://www.youtube.com/watch?v=nyMHBKlNk9c&pp=ygUVZXJpYyBwYXJrZXIgbW9kZGVkIG9z) which talks about the usage & risks of modded installs more in detail.

### Index
Here is a short outline of the things that will be covered in this guide.
- 1. Pre-Installation
- 2. OOBE
    - Bypass Microsoft Account Requirements
    - Force Local Account
- 3. Post-OOBE
   - Tools to run
   - Optional QoL Software

## Pre-Installation
There are two different ways to install Windows, it depends on personal preference. Before installing anything new, make sure to backup all your files on an external drive. It is reccomended to install Windows onto an NVME for the best performance. I use [this NVME](https://sabrent.com/products/sb-rocket-nvme4-1tb) but it's up to personal preference. <sub>This NVME in particular went on sale on Amazon for $49.</sub>

### Enterprise LTSC
The direct downloads for [Windows 11 LTSC is here](https://drive.massgrave.dev/en-us_windows_11_iot_enterprise_ltsc_2024_x64_dvd_f6b14814.iso) and the [Windows 10 version here](https://drive.massgrave.dev/en-us_windows_10_iot_enterprise_ltsc_2021_x64_dvd_257ad90f.iso). Since these are ISO files, you will need to burn it to a flash drive. I recommend using [Rufus](https://rufus.ie/en/) to do that. Enterprise LTSC is the best way to install as it removes additional bloat from your system and is overall more stable. LTSC does not get as many updates because it is meant for businesses who need a reliable version of Windows (think of IoT devices).

## OOBE

### Local Account Setup
In recent Windows feature updates, they force you to have an online account. They intentionally lock you out of making a local one during the initial setup but some smart people have figured out ways around this. Currently, the easiest way as of Windows 11 24H2 is to run a bypass command in the developer console. **Press <kbd>CTRL</kbd> + <kbd>SHIFT</kbd> + <kbd>J</kbd> to open the developer console** and then run `WinJS.Application.restart("ms-chx://LOCALONLY")`. You will now skip to the local account dialogue. Enter your desired username and password and proceed with the setup like normal. 

Make sure to turn off all of the boxes for Microsoft to collect your data, or switch them to minimal data collection. Don't worry as once we reach the desktop we can completely get rid of telemetry. Once all of that is done, you should finally be at the desktop!

## Post-OOBE
There are a few tools and commands that you should run and install first. This part is where everyone might forget to do or get stuck on. The first thing that I made sure to download was [O&O ShutUp 10++](https://www.oo-software.com/en/shutup10), [Remove MS Edge](https://github.com/ShadowWhisperer/Remove-MS-Edge), [Microsoft Activation Scripts](https://massgrave.dev/) (optional), and [Chris Titus Winutils](https://github.com/ChrisTitusTech/winutil). All of these play a crucial role in fine tuning your new Windows experience. If you want to tweak these yourself, skip to the next category. 

### O&O ShutUp 10++
If you want to use my configuration file, it's in the repository and [you can download it here](https://github.com/byeoon/Proper-Windows-Reinstall/blob/master/Byeoon%20OOSU10%20Config.cfg). To apply the changes, go to `File > Import Settings` and then select the config file you just downloaded. This removes all telemetry and additional system tracking. Feel free to adjust it to your own liking. 

### Optional Quality of Life Software
There are some other tools that may help you adjust Windows to your liking. [Winaero Tweaker](https://winaero.com) is one that I personally use on every reinstall because it has a bunch of customizable features and useful settings such as verbose logon messages and adding custom items to the context menu. Another nice quality of life customization tool that I use is *Add Name Here, I Forgot.*

#### Customization / Themes





