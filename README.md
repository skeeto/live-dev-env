# Live system of my personal config

## Download

 * [live-skeeto-20130805.iso](http://nullprogram.s3.amazonaws.com/iso/live-skeeto-20130805.iso)
   ([asc](http://nullprogram.s3.amazonaws.com/iso/live-skeeto-20130805.iso.asc))

### Previous versions

 * [live-skeeto-20130718.iso](http://nullprogram.s3.amazonaws.com/iso/live-skeeto-20130718.iso)
   ([asc](http://nullprogram.s3.amazonaws.com/iso/live-skeeto-20130718.iso.asc))
 * [live-skeeto-20130616.iso](http://nullprogram.s3.amazonaws.com/iso/live-skeeto-20130616.iso)
   ([asc](http://nullprogram.s3.amazonaws.com/iso/live-skeeto-20130616.iso.asc))

## Description

This live system has my favorite packages and configuration, including
all of my personal dotfiles, and is configured to boot into exactly my
preferred development environment.

 * https://github.com/skeeto/dotfiles
 * https://github.com/skeeto/.emacs.d

See the README files in each for all of the keybindings and features.
One of the core features is that the window manager can be completely
and conveniently driven without a mouse.

## Building the system

It's built using Debian's [live-build](http://live.debian.net/). The
configuration assumes you have a local mirror hosted on port 3142
(i.e. apt-cacher-ng). On Debian, or any Debian derivative, install
*live-build* and run these command from the repository.

    lb config
    sudo lb build

Root permissions are needed due to live-build's chrooting. The build
output will be called `binary.hybrid.iso`.

## Motivation

 * [Personal OS Configuration Live System](http://nullprogram.com/blog/2013/06/17/)
