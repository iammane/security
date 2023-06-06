# Windows Setup Guide

## Intro

Putting this together to highlight setting up a Windows machine to be used for ethical hacking / penetration testing **without** needing to install a VM in software such as Virtual Box or VMware.

The main justification for something like this is primarily speed and ease of use. There are tradeoffs though and anything that needs to be pointed out will be. This serves as a personal guide more than anything else but please feel free to use or suggest improvements!

## Initial Steps

First follow the steps here [Install WSL | Microsoft Learn](https://learn.microsoft.com/en-us/windows/wsl/install). This should be done prior to anything else. Run whatever updates are needed, reboot, just ensure the Windows Subsystem for Linux is installed and ready to go.

Once WSL is installed you have to install the distro of your choosing. You can actually do this in the Windows Store or from an admin PowerShell prompt (not covered here). For my purposes I'm installing the Kali Linux distro but truthfully any will work fine (Ubuntu, etc). Find your particular flavor in the Microsoft Store and click install. 

After the installation is completed you can run it - you'll be prompted to set up a username and password. It can match your Windows credentials, but it doesn't have to necessarily.

You should at this point be looking at a Linux prompt (from this point forward we'll assume Kali). Congratulations! 🎉 The initial setup is complete!

## Installation Items

The WSL version of Kali comes relatively bare bones. Luckily (in my testing at least) most tools can be installed separately and even ones with GUIs work! Before diving into any extra tools be sure to run a quick `sudo apt update` and `sudo apt upgrade`. Once that's set you'll want the following:

### Linux Installs
1. [GIT](https://git-scm.com/) - I can't remember if it's there or not, I don't think so. Simply run `sudo apt install git` and you're off to the races.
2. [Legion](https://github.com/GoVanguard/legion) - This tool is a good combo of NMAP scanning + Hydra, brute forcing, screen shotting. It's a nice one stop shop with a GUI. `sudo apt install legion`. The cool part about this one is that once you invoke it you actually get the graphical window on your Windows desktop. **It must be run with sudo, ie, `sudo legion`**
3. [Spiderfoot](https://github.com/smicallef/spiderfoot) - This is a pretty decent tool for OSINT gathering. In all honesty, I haven't had a lot of luck with it, but I suspect it's mostly in my usage (or lack of understanding). `sudo apt spiderfoot`.

### Windows Installs
1. JSON Viewer Pro
