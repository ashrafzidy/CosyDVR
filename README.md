CosyDVR
=======

An Android open souce car blackbox DVR app (GPLv3+)

<a href="https://f-droid.org/packages/es.esy.CosyDVR/" target="_blank">
<img src="https://f-droid.org/badge/get-it-on.png" alt="Get it on F-Droid" height="80"/></a>
<a href="https://play.google.com/store/apps/details?id=es.esy.CosyDVR" target="_blank">
<img src="https://play.google.com/intl/en_us/badges/images/generic/en-play-badge.png" alt="Get it on Google Play" height="80"/></a>

Features:
- Free and open source project forever
- Works in background as a service
- Works even when the keyboard is locked
- Autostart recording option after program launch
- Autoremove old files
- Simple placing files to favorite folder (one file or all files after current)
- FLASH button for night recordings (if device supports)
- Supports Android 4.1.2 (Fly IQ451 primarily tested)
- GPS data is recorded into subtitle files *.srt
- Separate *.gpx file for upload to the OpenStreetMap.org
- GPS data is shown on the screen
- Night mode for better video under low light condition (if device supports)
- Different focus modes (infinity, auto, continuous video, macro)
- Zooming in/out  with gestures
- Refocus on screen tap
- Exit function is protected with long click to avoid accedental click
- Configurable options (video size, bitrate, maximal temporary and minimal free space, fragment time etc.)
- Notification area clickable icon for bringing app to front
- Custom SD_Card_Path option
- Ukrainian, Russian, English, Italian, German interfaces
- Show battery level when device is not charging
- Time Compression (Time Lapse) function

Supported devices:
- Fly IQ451
- Prestigio PAP4055
- ASUS ME173X
- Samsung SM-GT310

Operation manual:
---

**Buttons:**

FAV - preserve current fragment from deletion (add to favorites).

        0 - this is temp fragment
        
        1 - this and all next fragments are preserved
        
        2 - only this fragment is preserved. Next will be temp
        
Restart - break fragments. Start new one

Restart (long click) - options menu

Focus - switch between focus modes (visible only supported by device)

        i - infinity
        
        v - continuous video
        
        a - automatic with manual autofocus
        
        m - macro with manual autofocus
        
        e - extended depth of field
        
FLASH - toggle flash on/off

Night - toggle night mode on/off. On long click - Time Compression Function On/Off. It uses
	Time Compression Factor from preferences.

Exit - exit application (exit on long click for eliminate accidental press)

**Gestures:**

Tap on screen - autofocus in "a" and "m" modes

Pinch screen - zoom in/out


Build Intructions under linux
---
  * Install toolchain

  `sudo apt-get install ant openjdk-8-jre openjdk-8-jdk`
  
  * Download and update SDK
  
  `wget http://dl.google.com/android/android-sdk_r24.4.1-linux.tgz`
  `tar -zxf ./android-sdk_r24.4.1-linux.tgz`
  `cd linux-sdk-tools`
  `tools/android update sdk --no-ui`
  
  * create project for ant
  
  `~/android-sdk-linux/tools/android update project -p . -t android-21 -n CosyDVR -s`
  
  * compile created project
  
  `ant debug`
  
  * install compiled debug version of project
  
  `ant installd`
  
  * debug with adb logcat

  `adb logcat | grep CosyDVR > logcat.txt`

  * check available devices with adb
  
  `adb devices`
  
  More info: http://developer.android.com/sdk/index.html#Other 

License:
---
        This program is Free Software: You can use, study share and improve it at your will. 
        Specifically you can redistribute and/or modify it under the terms of the 
        GNU General Public License as published by the Free Software Foundation, 
        either version 3 of the License, or (at your option) any later version.

