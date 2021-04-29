# fotoresize

Most camera devices take images with a much higher resolution than is necessary or practical for sharing or posting on the web.

This script accepts either a file or directory as an argument, it then downsizes the file or all image files in the directory so that their width and height do not exceed a certain size, defined in pixels.

The script checks to make sure that the files it processes are single-frame image files (e.g. are not GIFs) and then checks to see if they are already below the specified maximum width and height values.


## Configuration

No configuration needs to be done by default.

The maximum width and height are set to 1600x1600 and can be changed be editing the `maxW` and `maxH` values in the script.

Rescaled images have a tag appended to their file name.  The tag can be customized by changing the `tag` value in the script.


## Credits and Thanks

This script relies on the excellent [ImageMagick](https://imagemagick.org/) image software suite.

This script will run in any BASH shell on a system that has ImageMagick installeed including Linux, Cygwin-Windows, and OSX.


## Usage: 
```
fotoresize <file>|<directory>
```

## To Do

Right now the directory processor only accepts png and jpg files.  If there are other image types that would would like included please contact me.
