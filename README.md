# xboxdrv-mouse

This is a repository for a few settings for the xboxdrv driver, as it is used on a Fedora 24 - meantime Fedora 28 - Linux system. I didn't write this driver - its now read-only home was here:

* https://github.com/xboxdrv/xboxdrv

   The driver here is used for an Xbox 360 wireless controller (*1*), and for a German QWERTZ keyboard layout. And with xboxdrv this controller basically was turned into a mouse, or better: a remote control - with more than 20 buttons. Seems to work like a charm so far with very few, it seems, basically neglegible glitches. Currently it is used mainly for running mpv (*2*), the movie player. If you're used to handle joysticks you might even like to use this controller for navigating your desktop. And no: you can't type a full text with it. Not yet ... ;=)

   The problem lies with the documentation: I basically got the driver running via trial and error. So hopefully this situation can be changed with a little attention to the docs that already come with the driver itself, and some description of how I got it working.

To get the driver running you may want to start with something like that:

xboxdrv -s -c /path/to/mpv.mouse.xboxdrv

You find mpv.mouse.xboxdrv in the directory above.

And you might need something like input.conf for mpv, in the mpv folder above.

Enjoy!


----
* *1*  http://support.xbox.com/en-US/xbox-360/accessories/controllers
* *2*  https://github.com/mpv-player/mpv/releases
