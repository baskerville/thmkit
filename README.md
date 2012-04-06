This is a set of tools aimed at producing high quality color schemes.

It uses the **ANSI redefinition** technique to allow live color scheme switching and versatile themes (the same theme can be used with different color schemes).

At the moment, it works with `urxvt` (the required patch is `rxvt_unicode_xres256.diff`).

The main script is `genthm` which takes the hex value of the background color as first argument and the scheme name as optional second argument (run `genthm` without arguments to get the usage), it requires `Python` and the `python-colormath` library.

Once called it will output three files in the current directory: all those files except the vim theme shall be placed in `$XDG_COLORS_DIR` for the scripts in `extra/` to work.

[Preview](http://ge.tt/23u6FNC/v/3)
