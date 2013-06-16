# Live system demo of my personal configuration

This live system has my preferred packages, includes all of my
personal dotfiles, and is configured to boot into exactly my preferred
development environment.

 * https://github.com/skeeto/dotfiles
 * https://github.com/skeeto/.emacs.d

It's built using Debian's
[live-build system](http://live.debian.net/). The configuration
assumes you have a local mirror hosted on port 3142 (i.e.
apt-cacher-ng).

## Building the system

On Debian, or any Debian derivative, install *live-build* and run
these command from the repository.

    lb config
    sudo lb build

Root permissions are needed due to live-build's chrooting. The build
output will be called `binary.hybrid.iso`.
