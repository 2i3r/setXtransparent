# setXtransparent - set x window transparent

Simple script to make current x window (mostrly *gnome-terminal*) transparent.

This basically forked from [@nirbheek](gist.github.com/nirbheek.5589105) gist repository.

Here this script automatically find focused window and make it transparent to the percent sent to script by parameter `n` or has been writen to `~/.transparency` file. 

## Usage

First make it executable by `chmod +x setXtransparent` if it's not. then:
```
./setXtransparent n
```

Where n is chosen from `0-100`, `0` is complete transparent and `100` is solid color, 

You may also copy it to a path directory and run by:
```
setXtransparent n
```
you can go further and set your desired transparency percent by writing to `~/.transparency`, and then:
```
setXtransparent
```
is enough to set the current gnome-terminal transparent to your desired level.

### To do:
- If you put this command in `~/.profile` for some reason, when a new `gnome-terminal` starts, it won't get the correct `window id`, so trasnparency command may not set to the newly created window. 
- It's good to be able to run this command using keyboard shortcut, then it can be used faster and on more types of window (firefox, editors, etc). but when this script runs using keyboard shortcut, it fails to get correct `window id`, may be because it should be run as root to get that type of information?! in while it good to add option for user to select window using mouse click an `xwininfo` or ...

**_License_**: _BSD_
