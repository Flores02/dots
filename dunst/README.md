I have a quite odd [dunst](https://dunst-project.org) setup. The file [dunst/mondo](https://budrich.github.io/dots/dunst/mondo) is generated with [mondo](https://budrich.github.io/mondo) and contains the color definitions for dunst. By default i merge the mondo file with [dunst/lo-bar](https://budrich.github.io/dots/dunst/lo-bar) . But I have a [script](https://budrich.github.io/scripts/misc/dunst-layout) that can merge the mondo file with a different file and by doing so creating a temporary alternative notification layout.

# lo-bar

This layout displays a notification that only contains the summary (*%s*) in one line. It has the same height as my [polybar](https://budrich.github.io/dots/polybar/budbar) and it overlies the center of the bar when visible.  

# lo-rofi

This displays a multiline notification and is by default positioned in the top left corner under the statusbar. It is great for displaying verbose messages while getting userinput with rofi or dmenu.
