# xboxdrv-mouse

This is a repository for a few settings for the xboxdrv driver, as it is used on a Fedora 24 - meantime Fedora 29 - Linux system. I didn't write this driver - its now read-only home was here:

* https://github.com/xboxdrv/xboxdrv

   The driver here is used for an Xbox 360 wireless controller (*1*), and for a German QWERTZ keyboard layout. With a different keyboard maybe have a look at the `mpv.mouse.xboxdrv` file above, and if necessary try to change it accordingly.
   
   With the two config files in this directory the xboxdrv driver basically turns this controller into some sort of remote control - with more than 20 function keys. Currently it is used here mainly to navigate mpv (*2*), the movie player. 
   
   Watching movies or videos with the driver set-up like this will let you fast/slow forward or backward the video, switch on/off or change subtitles, change available languages or switch them off completely, slow down or increase playback-speed. You can watch the video upside-down or on one of its sides, and quite a bit more. Have a look at the config files, try the driver, and you probably never go back navigating a video with a keyboard.

To get the driver running maybe try starting with something like this:

*xboxdrv -s -c /path/to/mpv.mouse.xboxdrv*

Again: please see the `mpv.mouse.xboxdrv` file on top of this page.

And you might need something like `input.conf` for mpv, as the one in the mpv folder above.

Enjoy!


* _Update 2019-05-25:_  
      Uploaded a changed *mpv.mouse.xboxdrv* - unwanted mouse movements should now be stopped by higher `x{1,2}^dead` and `y{1,2}^dead` values.  



----
* *1*  http://support.xbox.com/en-US/xbox-360/accessories/controllers
* *2*  https://github.com/mpv-player/mpv/releases
