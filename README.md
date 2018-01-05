# bspwm-dotfiles
 my config for bspwm, tint2, dmenu and lxterminal.
 to install, see the blow.
# screenshots
![screenshot](bsp.jpg?raw=true "Title")
![screenshot](bsp2.jpg?raw=true "Title")
# installation
simply , try
```bash
git clone http://github.com/mmjafari.bspwm-dotfiles
cd bspwm-dotfiles
./install.sh
```
# usage
command | use
--------|--------
super + d | application menu
super + enter | lxterminal
super + alt + q | exit session
super + {t,T,s,f} | focused window condition modifier
super + m | should goto next desktop, but doesn't :))
super + {0..9} | goto desktop
super + w | close corrent window
super + q | same do.[1]
click | focuse [2]

note:
 1 - change this line(sxhkdrc):
 ```bash
 bspc node focused --close
 ```
 to that:
 ```bash
 bspc node focused --kill
 ```
 this will kill windows, grouping by app name.
 
 2. it's focusing by click. you can change it's value to false in bspwmrc
 
 3. battery applet doesnot working :)
