# Intro

These scripts allow you to set wallpapers with [Superpaper](https://github.com/hhannine/superpaper) on wlroots compositors with tools like:

- [hyprpaper](https://github.com/hyprwm/hyprpaper)
- [swaybg](https://github.com/swaywm/swaybg)
- [wpaperd](https://github.com/danyspin97/wpaperd)

## superpaper-set-hyprpaper

POSIX shell script

Depends on:
- hyprctl
- [ImageMagick](https://imagemagick.org/script/convert.php) convert

## superpaper-set-sway

Python3 script (no external libraries required)

Depends on:
- python3.11 
- [ImageMagick](https://imagemagick.org/script/convert.php) convert

Communicates with Sway over a socket

Note: Not able to give proper attribution (at this moment),
as I could not find the author of the script, on which this is based on.

# Setup

In order to use these scripts, you need to modify your Superpaper settings.

Open ~/.config/superpaper/general_settings in your favourite text-editor
and change/аdd (if missing) the line "set_command".

For example:

If you intend to use [hyprpaper](https://github.com/hyprwm/hyprpaper), you should set it to:

> set_command=superpaper-set-hyprpaper {image}
