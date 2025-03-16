# Proper Windows Reinstallation Guide <a href="https://ko-fi.com/byeoon">![Buy](https://img.shields.io/badge/Buy%20me%20a%20coffee!-byeoon-blue)</a>
**This guide is still being updated! Please be patient.**

The correct way to reinstall Windows. This guide helps power users reconfigure a fresh system to squeeze out as much performance and user safety as possible. This is a guide made for Windows 11, but most parts are backwards comaptible.

### Index
Here is a short and sweet outline of the things that will be covered in this guide. It is recommended to read EVERYTHING though!
- 1. Pre-Installation
  - World Mode
- 2. Installation / OOBE
    - Bypass Microsoft Account Requirements
- 3. Post-OOBE
   - Tools to run
   - Optional Software for QoL
   - Mod your apps
 

## Pre-Installation
Before installing Windows (10/11) while you are still in the media creation tool for the least amount of bloatware **SET YOUR REGION TO American (World)**. You may have to **uncheck** `Automatically set PC Defaults` or some box like that first. I cannot stress this enough because it will remove so much initial bloat. This removes any 3rd party applications that Windows tries to install on boot (For example, candy crush, tiktok, solitaire) and leave your computer an almost blank slate. Some services like the Microsoft Store will still be installed, but it can be removed later.

## Installation / OOBE
Of course, before installing, make sure to backup all your files on an external drive. Also, install Windows onto an NVME for the best performance. I use [this NVME](https://sabrent.com/products/sb-rocket-nvme4-1tb) but to be honest it's up to personal preference. <sub>Mine in particular went on sale on Amazon for $50, so try to find deals like that.</sub>

If you followed the first part properly, you will see this when booting into the OOBE ![OOBEREGION](https://github.com/user-attachments/assets/540035b5-ae64-4644-b8cb-650da28e7840)

This means you set the region to **American (World)** and the bloat will not be installed! Great! You are already closer to a better Windows.

### Local Account Setup
In recent Windows updates, they try to push you to have a permanently online account. They intentionally lock you out of making a local one during the initial setup but some smart people have figured out ways around this. Currently, the easiest way as of Windows 11 24H2 is to run a command in the internal developer console. **Press <kbd>CTRL</kbd> + <kbd>SHIFT</kbd> + <kbd>J</kbd> to open the developer console**. Once this is open, run `WinJS.Application.restart("ms-chx://LOCALONLY")`. You will now get pop up for creating a local account, enter your desired username and password and proceed with the setup like normal. 

Make sure to turn off all of the boxes for Microsoft to collect your data, or make them as optional and minimal as possible. Don't worry though, as once we reach the desktop we can completely get rid of telemetry. Once all of that is done, you should finally see your desktop!

## Post-OOBE


