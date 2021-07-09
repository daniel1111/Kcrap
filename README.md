# Kcrap Debian package

This repository builds a Debian package for [Kcrap](http://www.spock.org/kcrap/) - Kerberos Challenge-Response Authentication Protocol daemon. Amongst other things, Kcrap allows MSCHAPv2 authentication via MIT FreeRADIUS, see [this blog post](https://fuhry.com/blog/2012/01/01/mschapv2-against-mit-kerberos-yes-you-can/). The sources were originally taken from:
* http://www.spock.org/kcrap/kcrap-0.2.3.tar.gz
* https://aur.archlinux.org/cgit/aur.git/snapshot/kcrap.tar.gz - miscellaneous patches to make it compile 

## Building

There's a [Vagrantfile](https://www.vagrantup.com/docs/getting-started/), so just run 'vagrant up' to build the packages for Debian/Buster/amd64.

