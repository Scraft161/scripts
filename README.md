# scripts
a collection of scripts I wrote to ease my life

## List of scripts

### initcord
a simple shell script to install discord with OpenAsar and kernel

OpenAsar can be configured at `~/.config/discord/settings.json` [more info](https://github.com/GooseMod/OpenAsar#config)  
Kernel config is at `/etc/kernel-mod/` and is symlinked to `~/kernel-mod/`  
Some usefull kernel modules can be found [here (Discord channel)](https://discord.com/channels/891039687785996328/899717501120806963).

Only works on Arch Linux

### record
simple script to reinstall OpenAsar and kernel for when discord fucks your client mods up.
relies on an existing installation that has been initialized with `initcord`

Only works on Arch Linux

### multilaunch
simple bash script that uses dmenu and multimc(/polymc) to launch instances for you.

add/edit instances by editing the array at line 11

### scriptmenu
simple sh script that goes through your scripts in `~/scripts/` and runs the selected one.

Config is in `~/.config/scraft/config/scriptConfig` which should be a posix shell script that declares variables.  
This script will look for `SCDF_SelectionTool` and expects one of the following:

- dmenu
- rofi
- xprompt

a selection tool can also be passed as command-line argument in which case the config file is not used.

---
# Contributing
I guess you just PR like usual.
