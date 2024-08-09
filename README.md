# IP Webcam Linux client

An unofficial Linux client for the [IP Webcam](https://play.google.com/store/apps/details?id=com.pas.webcam) app on Play store.

# Requirements

- `adb`
- `v4l2loopback`
- `ffmpeg`
- On Arch based systems, you'll also need to install `android-udev` so you can use `adb` without root.

If you have an Arch based system (Arch/Manjaro), you can just do `sudo pacman -S android-tools v4l2loopback-dkms ffmpeg android-udev --needed` in terminal and you're good to go.

# How to use

- It is recommended to put this file in PATH, so you can call it from the terminal from everywhere.
- Just run `ipcam` in a terminal, enter the root password (`v4l2loopback` requires it), and keep the ffmpeg process running until you are done.
  - When you are done, press `Q` while in the terminal to stop the ffmpeg process.
- You can also use `ipcam-mpv` to open up the camera feed in the mpv player. You could also window share this on Discord.
- IP Webcam has a web interface you can access with a browser, after you run one of the scripts and it forwards the port via adb, you can go to [127.0.0.1:8080](https://127.0.0.1:8080) to access it.

# Connect over wifi

- Connect both the devices over the same network and start the server on mobile.
- Run this script and enter the **IP Address** of the network when promped [Leave blank if same].
- `adb` Dependency won't be needed for this.
