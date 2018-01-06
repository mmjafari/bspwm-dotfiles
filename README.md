# bspwm-dotfiles
 my config for bspwm, tint2, dmenu and lxterminal.
 to install, see the blow.
# screenshots
![screenshot](wm.jpg?raw=true "Title")
![screenshot](wm2.jpg?raw=true "Title")
# installation
simply , try
```bash
git clone http://github.com/mmjafari.bspwm-dotfiles
cd bspwm-dotfiles
./install.sh
```
after that, change this line:
```bash
~/.config/bspwm/bspwmrc
-------------------------
...
feh --bg-scale (path to your wallpaper)
```
# usage
command | use
--------|--------
super + d | application menu
super + enter | lxterminal
super + alt + q | exit session
super + {t,T,s,f} | focused window size modifier
super + m | should goto next desktop, but doesn't :))
super + {0..9} | goto desktop
super + w | close corrent window
super + q | same do.[1]
super + {h,c} | change fucesing
click | focuse [2]

note:
 1 - change this line:
```bash
~/.config/sxhkd/sxhkdrc
-----------------------------
bspc node focused --close
```
 to that:
```bash
~/.config/sxhkd/sxhkdrc
-------------------------
bspc node focused --kill
```
 this will kill windows, grouping by app name.
 
 2. it's focusing by click. you can change it's value to false in bspwmrc
 
 3. battery applet doesnot working :)
