# JackGrabbit
Mass Windows credential stealer payload for the BashBunny
TL;DR - Windows credential stealer for a TON of different accounts including slack, filezilla, windows passwords (local, cahced, and domain accounts if applicable), terminal server sessions, outlook,  many different browser's stored PWs, SSH keys and other authentication certificates, WiFi profile passwords (encrypted and plain-text), many many more, etc.

# Credit goes to illwill (first and foremost) / Hak5Darren / RazerBlade /
# This is a mix payload that will be expanded upon, so I am not removing the original Author's description; but not everything written inthe description is done by the payload. Many items will be borught in and merely commented out until they are ready for primetime.
# Title:         JackRabbit
# Author:        illwill
# Version:       0.1
#
# Jacks the Browsers/Windows/WiFi/SSH passwords and install config files from Windows boxes by downloading a 
# Powershell script into memory then stashes them in /root/udisk/loot/JackRabbit/%ComputerName%
#
# Credits to these guys for their powershell scripts:
# https://github.com/sekirkity/BrowserGather BrowserGather.ps1
# https://github.com/EmpireProject/Empire    Get-FoxDump.ps1
# https://github.com/fireeye/SessionGopher   SessionGopher .ps1
# https://github.com/gentilkiwi/mimikatz     md.ps1 from gentilkiwi/clymb3r/mattifestation obfuscated to mimidogz
#################################################################################################################
# Title:         USB Exfiltrator
# Author:        Hak5Darren
# Version:       1.1
# Target:        Windows XP SP3+
# Props:         Diggster, IMcPwn
# Category:      Exfiltration
# 
# Executes d.cmd from the selected switch folder of the Bash Bunny USB Disk partition,
# which in turn executes e.cmd invisibly using i.vbs
# which in turn executes and if stated, copies documents to the loot folder on the Bash Bunny.
#################################################################################################################
# PasswordGrabber

* Author: RazerBlade
* Creds: Hak5Darren, AlessandroZ
* Version: Version 1.1
* Firmware support: 1.1
* Target: Windows

## Description

Grabs password from all sort of things: chrome, internet explorer, firefox, filezilla and more...
This payload is quick and silent and takes about 3 seconds after the Bash Bunny have started to quack.
Full read here: https://github.com/AlessandroZ/LaZagne


## Configuration
By default the payload is identical to the Payload [usb_exfiltrator] but adds some commands to execute LaZagne and save the passwords to the loot folder.
I have commented out the copy command but if you want copy command and password just remove the remove infront of xcopy

Hak5 is not responsible for the execution of 3rd party binaries. Therefore I am not allowed to include it in github. You can easily download the binary from here or compile yourself https://github.com/AlessandroZ/LaZagne
When compiled or downloaded, just drop it of to the PasswordGrabbers folder and you are good to go!

Supported software

The LaZagne project
https://github.com/AlessandroZ/LaZagne/blob/master/pictures/softwares.png
(*) used by many tools to store passwords: Chrome, Owncloud, Evolution, KMail, etc.


