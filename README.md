# IP Webcam Linux client
Linux client for the [IP Webcam](https://play.google.com/store/apps/details?id=com.pas.webcam) app on Play store.

# Requirements
+ `adb`
+ `v4l2loopback`
+ `ffmpeg`
+ On Arch based systems, you'll also need to install `android-udev` so you can use `adb` without root.

If you have an Arch based system and have `yay` installed, you can just do `yay -S adb v4l2loopback-dkms ffmpeg android-udev` in terminal.

# How to use
+ It is recommended to put this file in PATH.
+ Just run `ipcam` in a terminal, enter a root password (`v4l2loopback` requires it), and keep it running until you are done.
+ You can also use `ipcam-mpv` to open up the camera feed in the mpv player. You could also window share this on discord.
+ IP Webcam has a web interface you can access with a browser, after you run one of the scripts and it forwards the port via adb, you can go to [127.0.0.1:8080](https://127.0.0.1:8080) to access it.
