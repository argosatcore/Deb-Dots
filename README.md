# Deb_Dots
⢀⣴⠾⠻⢶⣦⠀  
⣾⠁⢠⠒⠀⣿⡁  
⢿⡄⠘⠷⠚⠋⠀  
⠈⠳⣄⠀⠀⠀
   
---     

At the kernel of my computing milieu, there are two irreducible components: the [Debian GNU/Linux Operating System](https://www.debian.org/), as a solid foundation to build on, and the [awesome] window managar, as one of the most flexible and extensible frameworks to manage what probably is both, the most common ways of interactaing with with computers, and, simultaneously, one of its less examined aspects: the layout of the computing space.<sup>1</sup>
 
   The layout for this README.md was heavely influenced by that of [Spencer Tipping](https://github.com/spencertipping/dotfiles). Also, he (along with some [contributors](https://github.com/spencertipping/ni/graphs/contributors)) created an amazing tool for data processing pipelines in bash called [**_`ni`_**](https://github.com/spencertipping/ni). You should definetively check it out.
 
   These dot files were started with a minimal Debian 10 Buster installation, so they should work with any Debian installation or Debian-based distribution. 
     
   It is worth mentioning that although I use these dots on Debian, I've made an effort to keep them as distribution agnostic as possible. I have managed to deploy them succesfully in other distributions, especifically on [Arch Linux](https://archlinux.org/) (_btw_) and [Void Linux](https://voidlinux.org/). 

   If you find any of this useful, feel free to grab any part or all of it.
   
   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

1. In the recent past, I used [bspwm](https://github.com/baskerville/bspwm) as my default window manager. I still regard it as one of the best tiling window managers out there, but I found in awesome some features that made the switch worthwhile like the use of tags instead of workspaces (a word that, like the so called "productivity", is a word I really hate), the extensibility provided by its use of the Lua programming language and the integration of an status bar as part of awesome. If you are interested in giving bspwm a try, you can take a look at my dotfiles. Alson, a far more comprehensive and rigurous source on running bspwm on Debina is a book written by the greek philosopher,[Protesilaos Stavrou](https://protesilaos.com/), apropiately called _[Prot's Dots For Debian](https://protesilaos.com/pdfd/)_. His writings and videos on free and open source software may be of interest to those who wish to examine, both technically and philosophically, what, for better or for worse, has become an inescapable aspect of contemporary life. 

 ---
 
 **Floating Layout** |  **Binary Space Layout**
:-------: | :-------:
![Screenshot from 2021-02-16 15-38-46](https://user-images.githubusercontent.com/64110504/108127531-f987b280-7070-11eb-9075-1f406b222c73.png) | ![Screenshot from 2021-02-16 15-37-13](https://user-images.githubusercontent.com/64110504/108127578-0dcbaf80-7071-11eb-9055-0297cc7d1eb3.png)
**Tiled + Floating Windows Layout** | **Rofi's modes**
![Screenshot from 2021-02-16 16-05-40](https://user-images.githubusercontent.com/64110504/108127628-24720680-7071-11eb-8504-49a7d652d007.png) | ![Rofimodi](https://user-images.githubusercontent.com/64110504/108127676-36ec4000-7071-11eb-9b05-57f046b326d7.gif)


## Unexpected features you get right out of the gate
- **Bash's vim mode:** When in _normal_ mode, you will see a `-` at the beginning of your prompt. When in _insert_ mode, you will see a `+` at the beginning of the prompt. 
- **Caps Lock key is swapped with Esc key:** Caps Lock has way too much of a good position in they keyboard for the function it provides. If you are a vim user (or someone that just uses the crap out of the Esc key), you know how handy this is. If you don't want this, just delete the `.speedswapper` file and/or comment out the corresponding line in the `.xsessionrc file`.
- **Mouse set for left handed people:** Because I'm a lefty. That's it. If you happen to be part of the other 90% of the human population, just delete the  `.mouseconfig` file and/or comment out the corresponding line in the `.xsessionrc file`.  
- **Change directories without using the `cd` command:** Just type the name of the directory to move into it. 
- **Bash completion is no longer case sensitive:** No more wasted time pressing keys to get upper case letters.
- **Combined less and neovim as a pager for man pages:** Because man pages deserve better.
- **Keyboard layout set to Latin American:** Unless you need to type Spanish accents, you might want to take a look at the `.xsessionrc` file and chage the keyboard layout to your preferred one. Probably changing  `latam` for something like `us_intl` will do the job.


## Stuff referenced by these configs
All of which are `apt install`able:

- `neovim`: text editor.
- `rxvt-unicode`: terminal emulator.
- `awesome`: window manager.
- `awesome-extra`: additional modules for awesome.
- `rofi`: application launcher, window switcher, commad executor and many more.
- `nautilus`: file manager.
- `dunst`: notifications daemon.
- `compton`: compositing for window transparency.
- `tmux`: persistent SSH shell sessions.
- `feh`: sets the desktop background.
- `i3lock`: screen locking.
- `redshift`: sets screen's temperature color according to time of day.


## (Some) keybindings

### List of keybindgs:
- `Super+Ctrll+r`: showo a complete list of keybindings. 

### Awesome:
- `Super+Ctrll+r`: reload awesome.
- `Super+Shift+q`: exit awesome session.
- `Alt+Ctrl+l`: lock screen.

### Tags:
- `Super+(left arrow key, right arrow key)`: move to the previous or next workspace. 
- `Super+(1,2,3,4,5,6,7,8,9,0)`: go to a desginated tag.
- `Super+Shift+(1,2,3,4,5,6,7,8,9,0)`: move an active window to a desginated tag.

### Windows:
- `Super+q`: close.
- `Super+f`: fullscreen. 
- `Super+Ctrl+space`: toggle floating. 
- `Super+n`: minimize.
- `Super+Ctrl+n`: restore minimized.
- `Super+r`: rotate windows clockwise.
- `Super+(h,j,k,l)`: change the selection of a window in a designated direction.
- `Super+Shift+(h,j,k,l)`: move window in a designated direction.

### Mouse:
- `Shift+click4`: float a tiled window and viceversa.
- `Super+click1`: move window.
- `Ctrl+click2`: resize window.

### Running things:
- `Super+Return`: run a terminal.
- `Super+Shift+Space`: run a terminal in a tmux session.
- `Super+i`: run firefox.
- `Super+a`: run nautilus.
- `Super+d`: run rofi as an application launcher.
- `Alt+Tab`: run rofi as a window switcher.
- `Super+e`: run rofi as a power menu. 
- `Super+w`: run rofi as a wifi menu.
