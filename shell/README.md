prompt

My prompt shows the runtime of the last command and a compact `CWD` (current work directory). 

[![](https://budrich.github.io/img/awd/ss_time4prompt.png)](https://budrich.github.io/img/org/ss_time4prompt.png)

-----

inputrc

These settings modify the behavior of manual input to the terminal. I use VI-mode and by setting:

``` text
set show-mode-in-prompt on
set vi-ins-mode-string
set vi-cmd-mode-string :
```
`:` is displayed at the beginning of the prompt when i am in *command* mode.

[![](https://budrich.github.io/img/awd/vimodesinprompt.gif)](https://budrich.github.io/img/org/vimodesinprompt.gif)

-----

The `read -rsn1 -t2 input` waits two seconds for a key-press before it starts **X** and **i3**. If I press `1` I stay in the wonderful tty environment. If I press `2` or wait 2 seconds, **i3** starts. o

I have found this method much more convenient then a normal DM, where you have to change DE from some, very easily forgotten, menu. Often resulting in me logging in to the wrong DE...

I also source all files in `~/.bash/` . I just upgraded Mint and it was kind enough to overwrite my `.bashrc`, that made me decide to have it as minimal as possible so I can easily restore it if something similar happens.

I don't care so much about GNU/Linux-distros and I have not had any problems with Mint till this happened. But it is so poor design to overwrite `.bashrc` that I'm seriously thinking on hopping just because of that.\* 

But maybe other distros behave similar...

\* *edit: i now run arch linux, and before that PeppermintOS*


My aliases. I add aliases with the function `adda` that is defined in [bash/func](https://budrich.github.io/dots/bash/func). Here you can find the famous `lolban` alias ;)

This is the power of the bash shell, you can write small functions to make using the shell easier. 

**lb**  
I found this one on the [LinuxBBQ forums](https://linuxbbq.org/bbs/viewtopic.php?f=4&t=2076) it adds the last command to a logfile. Very handy.

**adda**  
Adds a new permanent alias. Example:   
`adda dwn cd ~/Downloads`  
this will add, `alias dwn='~/Downloads'` to [~/.bash/alias](https://budrich.github.io/dots/bash/alias) and reloads [~/.bashrc](https://budrich.github.io/dots/bash/bashrc) so you can use the alias immediately. 

**apti/gemi/pipi**  
install packages and log package name.

**mcd**  
Classic function that creates a folder and cd into it.

-----
