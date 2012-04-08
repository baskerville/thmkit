This is a set of tools aimed at producing high quality color schemes.

At the moment, it works with `urxvt` (the required patch is `rxvt_unicode_xres256.diff`).

The main script is `genthm` which takes the hex value of the background color as first argument and the scheme name as optional second argument (run `genthm` without arguments to get the list of available options), it requires `Python` and the `python-colormath` library.

Once called it will create two files in the current directory. The one starting with `redef-` is executable and can change the terminal colors in real-time. The other file shall be fed to `xrdb`. You might want to look at the scripts in `extra/` to see how dark/light scheme switching can be automated.

[Preview](http://ge.tt/23u6FNC/v/3)
