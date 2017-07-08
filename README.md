# setXtransparent - set x window transparent

Simple script to make current x window (mostrly *gnome-terminal*) transparent.

This basically forked from [@nirbheek](gist.github.com/nirbheek.5589105) git repository.

Here this script automatically find focused window and make it transparent by the percent sending to script by parameter `n` or has been writen to `~/.transparency` file. 

## Usage

First make it executable by `chmod +x setXtransparent` if it's not. then:
```
./setXtransparent n
```

you may also copy it to a path directory and run by:
```
setXtransparent n
```
you can go further and set your desired transparency percent by writing to `~/.transparency`, and then:
```
setXtransparent
```
is enough to set the current gnome-terminal transparent to your desired level.

**_License_**: _BSD_
