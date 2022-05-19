# KURZSCHLIESSER-EV3DEV-CPP

This file is copypasted from [https://github.com/pinjuf/kurzschliesser-ev3dev](https://github.com/pinjuf/kurzschliesser-ev3dev)

## Getting started

### Requirements

 - some version of Linux for the EV3 (preferably [ev3dev's Debian](https://www.ev3dev.org/downloads/))
 - git
 - a robot similar to `robo_V1.io` (BrickLink Studio file)

### Setting up and running

 1) Follow the instructions on [ev3dev.org](https://www.ev3dev.org/docs/tutorials/connecting-to-the-internet-via-usb/)
 2) Mount the brick's filesystem: `mkdir $mountpoint; sshfs -o idmap=user robot@ev3dev.local: $mountpoint`
    > You will be asked a passwd, the default on ev3dev is `maker`
    >
    > `sshfs` requires the FUSE linux kernel module. It will not work on WSL 1 etc., which doesn't provide an actual kernel.
    > 
    > To unmount, use `fusermount -uz $mountpoint`
 3) CD into the Brick's FS: `cd $mountpoint`
 4) Clone this repo (git clone https://github.com/n-i-r-e-x/kurzschliesser-ev3dev-cpp)

 5) I need to translate the python code to C++ before I can write (copypaste) more
