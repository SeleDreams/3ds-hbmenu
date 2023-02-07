# The Homebrew Launcher - FOR DEVELOPERS

## WARNING 1 : This is not the standard homebrew launcher, this is a fork for homebrew developers.
## WARNING 2 : At the time of writing, you will need to install a fork of luma3ds in order to be able to use it.




This repository contains a fork of homebrew launcher specifically made for helping homebrew developers debug their homebrews.

You will however need a specific fork of luma to be able to use it. The reason being that at the time of writing, rosalina did not expose a way to communicate with it from third party homebrews.

I did submit a pull request here for the feature to end up in mainstream luma3ds but it is not yet the case https://github.com/LumaTeam/Luma3DS/pull/1836

You can find my fork here https://github.com/SeleDreams/Luma3DS

This version of the homebrew launcher communicates with luma to make it start the debugger when starting a homebrew software and if a 3dslink.txt file is present on the root of the sd card, it will automatically start 3dslink when it starts, making it way faster to get started with debugging homebrews. Even more if you replace the boot.3dsx at the root of your sd card and then in the luma config (sd:/luma/config.ini), set the autoboot_mode value to 1. Doing this will make homebrew launcher start on boot of the 3ds, so that if your homebrew freezes the whole console you can very quickly go back to debugging after rebooting

Original repository of homebrew launcher : https://github.com/devkitPro/3ds-hbmenu