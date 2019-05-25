# xboxdrv-mouse

This is a repository for a few settings for the xboxdrv driver, as it is used on a Fedora 24 - meantime Fedora 28 - Linux system. I didn't write this driver - its now read-only home was here:

* https://github.com/xboxdrv/xboxdrv

   The driver here is used for an Xbox 360 wireless controller (*1*), and for a German QWERTZ keyboard layout. With a different keyboard have a look at the *mpv.mouse.xboxdrv* file above, and if necessary try to change it accordingly.
   
   With the two config files in this directory the xboxdrv driver basically turns this controller into a mouse, or keyboard, or better: some sort of remote control - with more than 20 function keys. Currently it is used here mainly for running mpv (*2*), the movie player.

   The problem lies a bit with the documentation: I basically got the driver running via trial and error. So hopefully this situation can be changed with a little attention to the docs that already come with the driver itself, and some description of how I got it working.

To get the driver running maybe try to start with something like this:

*xboxdrv -s -c /path/to/mpv.mouse.xboxdrv*

You find the *mpv.mouse.xboxdrv* file in the directory above.

And you might need something like input.conf for mpv, as the one in the mpv folder above.

Enjoy!


* _Update 2019-05-25:_  
      Uploaded a changed *mpv.mouse.xboxdrv* - unwanted mouse movements should now be stopped by higher `x{1,2}^dead` and `y{1,2}^dead` values.  



----
* *1*  http://support.xbox.com/en-US/xbox-360/accessories/controllers
* *2*  https://github.com/mpv-player/mpv/releases
