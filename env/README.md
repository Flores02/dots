My environment dotfiles is where i setup my, well, environment. [i3env](https://budrich.github.io/dots/env/i3env) are environment variables that i have invented myself and most of them are settings for various **i3ass** scripts. I could have put them in `.bashrc`, but I source them from [~/.xinitrc](https://budrich.github.io/dots/env/xinitrc) since all of them are specific to a graphical environment.  

Similarly [export](https://budrich.github.io/dots/env/export) are environment variables that are sourced in [~/.bashrc](https://budrich.github.io/dots/shell/bashrc).   

I try to keep most of my xsession related always start executions in [~/.xinitrc](https://budrich.github.io/dots/env/xinitrc), such as `compton`, `urxvtd` and loading the `seba` keyboard layout. 

I also put the user-dirs dot file here because *I'm just a soul whose intentions are good
Oh Lord, please don't let me be misunderstood*.
