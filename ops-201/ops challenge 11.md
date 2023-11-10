# Ops Challenge - Automated Endpoint Configuration

**Date**: November 6, 2023

**Team**: Juan Miguel Cano, Jasmine Pressley, Festus Oguhebe, Scotty Jokon, Nico Watson, Rodolpho Gonzalez

## Overview

Standing up Windows 10 endpoints from scratch can be extremely time-consuming. You will want to automate Windows system configurations as much as possible to save yourself precious time. In class, we can simply export an OVA of a Windows 10 VM; however, in a production operations environment, you may not have such luxuries. It is good to get a sense of how PowerShell can contribute to this effort.

## Scenario

Your team wants to automate the system's configuration of new Windows 10 deployments.

## Objectives

Write a PowerShell script that automates the configuration of a new Windows 10 endpoint. Your script should perform the following:

- Enable File and Printer Sharing
- Allow ICMP traffic
- Enable Remote management
- Remove bloatware
- Enable Hyper-V
- Disable SMBv1, an insecure protocol

**Test and validate that your script achieves the desired outcome for each listed objective. Put screenshots and discussion of your testing into a Google Doc and submit the link alongside your Github link.**

## Resources

- [Powershell one-liners](https://github.com/superswan/Powershell-SysAdmin)

## Tasks

Your script should perform the following:

```powershell
# Enable File and Printer Sharing
Set-NetFirewallRule -DisplayGroup "File And Printer Sharing" -Enabled True

# Allow ICMP traffic
netsh advfirewall firewall add rule name="Allow incoming ping requests IPv4" dir=in action=allow protocol=icmpv4

# Enable Remote management
reg add "HKLM\SYSTEM\CurrentControlSet\Control\Terminal Server" /v fDenyTSConnections /t REG_DWORD /d 0 /f

# Remove bloatware
iex ((New-Object System.Net.WebClient).DownloadString('https://git.io/debloat'))

# Enable Hyper-V
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All

# Disable SMBv1, an insecure protocol
Set-SmbServerConfiguration -EnableSMB1Protocol $false -Force
