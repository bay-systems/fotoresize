# fotoresize

I wrote this script due to the frequent need to downsize images for sharing and for posting on the web.  Most camera devices take images with a much higher resolution than is necessary or practical for sharing or posting on the web.

I wanted a simple script that will accept either an file or directory as an argument and will downscale the file or all image files withing the directory.

The script checks to make sure that the files it processes are single-frame image files (e.g. are not GIFs) and then checks to see if they are already below the specified maximum width and height values.

The maximum width and height are set to 1600x1600 and can be changed be editing the `maxW` and `maxH` values in the script.

In addition, rescaled images have a tag appended to their file name.  The tag can be customized by changing the `tag` value in the script.

This script relies on the excellent [ImageMagick](https://imagemagick.org/) image software suite.

This script will run in any BASH shell on a system that has ImageMagick installeed including Linux, Cygwin-Windows, and OSX.



## Usage: 
```
fotoresize <file>|<directory>
```

