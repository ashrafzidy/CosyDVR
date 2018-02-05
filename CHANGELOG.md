### v.1.3.21 (2018.02.05 23:19)

  * Bugfix: sizes of TEMP and FREE spaces are in kilobytes now

### v.1.3.20 (2017.07.06 16:36)

  * Default storage dir for Android 4.x =  ExternalStorageDirectory + "/CosyDVR"
  * Custom video rotation angle
  * Video rotation info in file metadata preference
  * Separated interface layout rotation from video rotation and rotation metainfo
  * Orientation parameters changes on the fly. No restart needed any more
  * Buttons with long click functions have hints now
  * Disable button hints option on help screen added

### v.1.3.19 (2017.06.29 11:54)

  * Fixed null dirs when there is no sd card present

### v.1.3.18 (2017.06.27 01:30)

  * SD Card detection improved for Adroid 5.x. Now ExternalMediaDirs and ExternalFilesDirs are detected
  * Not filtering tmpfs (ram drives) and other dirs like (obb, asec, secure etc) any more
  * Default storage dir is one from getExternalStorageDirectory, getExtrernalMediaDirs or getExternalFilesDirs

### v.1.3.17 (2017.05.26 12:44)

  * MIN_FREE_SPACE MAX_TEMP_SIZE are now parsed as truly long

### v.1.3.16 (2017.04.24 12:55)

  * Start/Restart button proper display with autostart off.
  * Preview of values in preferences
  * Default time compression value 6

### v.1.3.15 (2017.04.10 20:39)

  * Added japanese translation. Thanks to naofum <naofum@gmail.com> (https://github.com/naofum)

### v.1.3.14 (2017.03.13 12:51)

  * Fixed russian translation. Thanks to Alexey Vazhnov (https://github.com/vazhnov)

### v.1.3.13 (2016.09.20 11:20)

  * Fixed audiostream for normal video. Returned build.xml, project.properties etc for f-droid build system.y

### v.1.3.12 (2016.08.29 15:53)

  * Added experimental time lapse function (i.e. Capture Frame Rate is lower CompressTimeFactor times)
	TimeLapseMode is activated on nightButton LongClick. Video is restarted. Subtitles and GPX are
	collected at slower rate too. Thus one can use such mode while car is on the parking for long time.

### v.1.3.11 (2015.09.08 14:55)

  * Some minor fixes in English Preferences texts. Thanks to snelltheta

### v.1.3.10 (2015.06.15 09:15)

  * Added German interface thanks to Andy Dee <andi_d_@web.de>

### v.1.3.9 (2015.06.12 22:12)

  * Trying to fix KitKat SDcard issue. Now video is saved to [SDcard]/Android/data/es.esy.CosyDVR/fav or temp
  * Fixed preview orientation when there are no user defined preferences at all.

### v.1.3.8 (2015.06.10 19:30)

  * Refactored scanning storage resources

### v.1.3.7 (2015.05.31 09:45)

  * Fixed crash for devices without flash.

### v.1.3.6 (2015.05.12 20:04)

  * Added reverse landscape orientation option in preferences (needs to reinstall app or clear defaults)
    Reverse landscape mode is applied after application restart.

### v.1.3.5 (2015.05.11 20:04)

  * Added Italian translation thanks to fvasco
  * Renamed package to es.esy.CosyDVR

### v.1.3.4 (2015.04.21 16:29)

  * Added propagation of zoomfactor through fragments (Juan Jose Zamorano issue)

### v.1.3.3 ()

  * Fixed russian translation in order to implement Dmitry Lahoda patch.

### v.1.3.2 (2014.11.20 18:20)

  * Added preference to disable GPS usage

### v.1.3.1 (2014.11.18 11:15)

  * Fixed preferences english texts, added units in pref. dialogs on video parameters and so on
  * merged push request on README.md from asd-and-Rizzo

### v.1.3 (2014.11.13 20:11)

  * Fixed propagation of night mode, flash status and focus mode between fragments

### v.1.2 (2014.07.11 11:08)

  * Fixed autoclean temp folder
  * Added battery level indicator when device is not charging

### v.1.1 (2014.06.26 16:08)

  * Removed unnecessary permissions and features from AndroidManifest.xml
  * Added Help and About in preferences
  * Added Ukrainian interface
  * Added Russian interface

### v.1.0.6 (2014.06.25 16:17)

  * Added update FAV button during fragment split (to see if fav mode is on)

### v.1.0.5 (2014.06.24 11:50)

  * External SD_Card property now is list of available devices
  * Fixed camera initialization for Samsung SM-GT310
  * Fixed CosyDVR dir creation for Samsung SM-GT310
  * Added checking focus modes after start
  * Added checking supported scene modes (night/auto)

### v.1.0.4 (2014.06.23 15:12)

  * Fixed "Video Height" property

### v.1.0.3 (2014.06.20 17:25)

  * Fixed "Autostart Recording" property
  * Fixed "SD_Card_Path" property usage after program start

### v.1.0.2 (2014-06-13)

  * Added "Autostart Recording" property

### v.1.0.1 (2014-06-12)

  * Added preference "SD card destination path"
  * Simplified focus modes names (for devices with small screen)

### v.1.0 (2014-05-22)

  * First public version for inclusion to F-Droid repository
