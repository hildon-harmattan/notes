notes
=====

This repository contains a readme

The following are what I remember doing for getting hildon-desktop work on harmattan.

Sources list
------------
```
deb http://harmattan-dev.nokia.com/ harmattan/sdk free non-free
deb-src http://harmattan-dev.nokia.com/ harmattan/sdk free
deb http://harmattan-dev.nokia.com/ harmattan/41667a5bd857be02f487c2ce806fbf85 nokia-binaries

deb http://repo.pub.meego.com//home:/MartinK:/gtk/MeeGo_1.2_Harmattan_Maemo.org_MeeGo_1.2_Harmattan_standard ./
deb http://repo.pub.meego.com//home:/MartinK:/harmattan/MeeGo_1.2_Harmattan_Maemo.org_MeeGo_1.2_Harmattan_standard ./

deb http://repo.pub.meego.com//home:/ph5:/boost/Harmattan ./ 
```

I added the above sources to harmattan sdk and used whatever I could find so that I would avoid compiling it with the exception of GTK, as I wasn't sure if Cordia gtk had any significant changes.

Other packages 
---------------
I don't remember which packages come from where. I know I should have documented that but I didn't. When I encountered a dependency I tried to find the most easy way to compile. In general I used packages from the following projects in this order
1. Harmattan (meego obs)
2. Maemo (nokia or extras)
3. Debian
4. Upstream


Non-modified packages
---------------------

Some packages are needed but I have not modified them in any way from the cordia ones. Those do not exist in harmattan-hildon organization, and should be forked
1. gtk
2. hildon-home
3. hildon-status-menu



Other notes
-----------

I didn't manage to build gtk-doc for harmattan, but I overcame the obstacle by building everything else without gtk-doc support. However I did some things toward that goal so I am including my modified gtk-doc here (changes are only in the configuration and makefiles)

I have xrandr here in my dev folder but I'm pretty sure I didn't have to use it finally.


