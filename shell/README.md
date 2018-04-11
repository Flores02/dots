These are the dotfiles that configure my shell, currently I'm using `bash`.  

These files are sourced into `~/.bashrc`:

[shell/prompt](https://budrich.github.io/dots/shell/prompt) | prompt style and command
:---|:---
[shell/func](https://budrich.github.io/dots/shell/func) | small homebrew and borrowed functions
[shell/alias](https://budrich.github.io/dots/shell/alias) | alias file
[shell/path](https://budrich.github.io/dots/shell/path) | directories in `$PATH`
[shell/misc](https://budrich.github.io/dots/shell/misc) | other options and settings
[env/export](https://budrich.github.io/dots/env/export) | Environment variables


I also keep some settings in [shell/inputrc](https://budrich.github.io/dots/shell/inputrc), mostly keybindings and VI-mode options.  

And a few shell/terminal settings is defined in [xfiles/urxvt](https://budrich.github.io/dots/xfiles/urxvt)  

---------------


# prompt

My prompt shows the runtime of the last command and a compact `CWD` (current work directory). 

[![](https://budrich.github.io/img/awd/ss_time4prompt.png)](https://budrich.github.io/img/org/ss_time4prompt.png)

-----

# inputrc

These settings modify the behavior of manual input to the terminal. I use VI-mode and by setting:

``` text
set show-mode-in-prompt on
set vi-ins-mode-string
set vi-cmd-mode-string :
```
`:` is displayed at the beginning of the prompt when i am in *command* mode.

[![](https://budrich.github.io/img/awd/vimodesinprompt.gif)](https://budrich.github.io/img/org/vimodesinprompt.gif)

-----

# bashrc

The `read -rsn1 -t2 input` waits two seconds for a key-press before it starts **X** and **i3**. If I press `1` I stay in the wonderful tty environment. If I press `2` or wait 2 seconds, **i3** starts. o

I have found this method much more convenient then a normal DM, where you have to change DE from some, very easily forgotten, menu. Often resulting in me logging in to the wrong DE...

# func/alias

I add aliases with the function `adda` that is defined in [shell/func](https://budrich.github.io/dots/shell/func)  

### function descriptions:

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
