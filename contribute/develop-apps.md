---
layout: default
title: Develop apps for Linux/Ubuntu
description: 
---

# Develop apps for Linux/Ubuntu

There are all sorts of applications that are already made available through various package repositories, such as [apt](http://manpages.ubuntu.com/manpages/bionic/man8/apt.8.html), [The Ubuntu archive](https://packages.ubuntu.com/) provides debian packages that the system needs. On a brand new install of Ubuntu, this is the application delivery mechanism you are likely to use to install something.

Then came along “containerized” application models, such as [Snap](https://snapcraft.io/), [Flatpak](https://flatpak.org/), and [AppImage](https://appimage.org/). Let’s take a closer look at each of the types of packages and how you can get involved.


## Debian packages

Because Ubuntu is a Debian derivative, the historic package management software is set up to consume .deb packages, through various tools like dpkg and apt. If you are interested in packing your application as a .deb, then I suggest you take a look at [the Debian packaging wiki page](https://wiki.debian.org/Packaging).


## Snap

Snap is the application packaging system developed by Canonical and the corresponding snaps are typically deployed from [the snap store](https://snapcraft.io/store). 


### Building your own snaps

You can build snaps locally as well as on snap store build hardware (if you’d like to build your snap for a wider audience).

Head over to [the snapcraft documentation](https://snapcraft.io/docs) to learn more about building locally with the snapcraft build tool. This is a great way to iteratively test your snap application before you’re ready to release it.

When you’re ready to have the snap store disseminate your application, then consider linking your github repository to [the snapcraft build system](https://snapcraft.io/build).


### Contributing to snapcraft

If tinkering under the hood is The snapcraft team is always looking for improvements that help make the snap build system better than ever! Go check out [the snapcraft contribution guide](https://github.com/snapcore/snapcraft/blob/master/CONTRIBUTING.md). 


### Getting help with snaps

There is an active community that hangs out on [the snapcraft forum](https://forum.snapcraft.io/). 


## Flatpak

plop


## AppImage

plop
