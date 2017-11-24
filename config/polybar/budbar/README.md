
Polybar is a great statusbar that works well with i3 and other window managers, this is my config file. It uses some custom scripts to display some information.

[![](https://budrich.github.io/img/awd/"ss-17-11-22-pbarro.png")](https://budrich.github.io/img/org/"ss-17-11-22-pbarro.png")

In the screenshot above you can see polybar at the top of the screen. I use [i3fyra](/i3ass/i3fyra) to achieve the layout. Container A(vivaldi/wg) and B(irssi)  are tabbed and container C is horizontally split with three urxvt instances.

I use some custom scripts to display some of the information in my polybar.

|**script**|**function**|
|:-----|:-------|
|[pbmail](https://github.com/budRich/dots/tree/master/config/polybar/src/pbmail)    | shows the number of unread mails|
|[pbmic](https://github.com/budRich/dots/tree/master/config/polybar/src/pbmic)     | microphone volume|
|[pbvol](https://github.com/budRich/dots/tree/master/config/polybar/src/pbvol)     | output volume|
|[pbweather](https://github.com/budRich/dots/tree/master/config/polybar/src/pbweather) | shows what beautiful Swedish weather it is outside|
