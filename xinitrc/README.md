
This is part of my *anti-DM* suite. The stuff I want to happen just before i3 loads up, goes here. 

Starting `urxvt` in daemon mode is really nice and makes it consume less resources and spawn new terminal windows much faster.   

I use `hsetroot` to set the desktop background to a [minimal tiled pattern](https://github.com/dkeg/bitmap-walls) and use the background color from [Xresources](dots/xresources). 

The [Seba](https://budrich.github.io/blog/swedish_keyboards) keyboard layout keeps me sane! 

I also have some special options to `setxkbmap`. `lv3:ralt_switch` is needed to type swedish characters. `caps:ctrl_modifier` makes the `CapsLock` function like a extra `Ctrl`.

`xcape` is a really cool little program that can remap keys when they are tapped, but keep theire original function when they aren't. I use it to make my `CapsLock` key to act as `Esc` when it is tapped, VIM-users will understand.

I use `numlockx` to be sure that `NumLock` is activated.

I try to avoid using the mouse as much as possible, and my laptop has a trackpoint, so the touchpad is just annoying, the `xinput` command disables the touchpad. I found this article helpful to understand `xinput`:  

http:/https://budrich.github.io/blog.yjl.im/2010/12/using-xinput-to-disable-keyboard-mouse.html

I use `sxhkd` to [remap the back button of the mouse to backspace](https://budrich.github.io/blog/mouseback).

I used to use `unclutter` to hide the mouse pointer, but I found it broken. [xbanish](https://github.com/jcs/xbanish) is a much better alternative, but I had to download and compile it from source, since it's not in the ubuntu repositories. 

[compton](https://github.com/budRich/dots/tree/master/config/compton) compositor.
