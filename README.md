This is a set of tools aimed at producing high quality color schemes.

At the moment, it works with `urxvt` (the required patch is `rxvt_unicode_xres256.diff`).

The main script is `genthm` (run `genthm -h` to get the list of available options/arguments), it requires `Python` and the `python-colormath` library.

Once called it will create two files in the current directory. The one starting with `redef-`, once executed, will change the terminal colors in real-time. The other file shall be fed to `xrdb`. You might want to look at the scripts in `extra/` to see how dark/light scheme switching can be automated.

[Preview](http://ge.tt/23u6FNC/v/3)

# Vim Theme Skeleton Helper

To make vim aware of the special skeleton color syntax, put `extra/vim.vim` in `~/.vim/ftplugin/`.
