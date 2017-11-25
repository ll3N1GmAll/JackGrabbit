# JackGrabbit
Mass Windows credential stealer payload for the BashBunny

# Credit goes to illwill (fist and foremost) / Hak5Darren / RazerBlade /
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
