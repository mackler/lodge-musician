# Lodge Musician

This setup is based on [SoundShow](https://soundshow.app/getting-started)

Get it [here](https://soundshow.app/downloads)

You can extract it and run it from the extracted directory.

You can activate Pro mode with the license key from your email.

The configuration file is an `.ssp` file. Open it under the Project menu.

The configuration file refers to files in
`/usr/local/SoundShow-soundfiles/`. As you collect music, put the
prepared files under that directory. When you prepare a device for
performance you can use the same configuration file by putting the
sound files in a directory with the same name.

# Configuration and its limits

Apparently some parameters are not saved in the configuration file, so
you may have to set them each time the app is started.

In the left there are two buttons determining what the left and right mouse buttons will do. With a touchscreen you only have the left as far as I know. Best to leave left on "Toggle Fade"

"Next sound" volume defaults to 60. Try to remember to set volume to 100 for every sound file.

Enable fade in on every clip, but set time to zero, to override the default fade-in.

There are two ways to develop:

- Install SoundShow on the performance device, and update the config file and sound files to make changes.
- Create a bootable image and put it on a USB drive.

# Install SoundShow on the performance device

Have a USB for copying.

- Make a copy of the sound-files directories, and the config file on the USB drive.
- Copy onto the device.

Put the SoundShow directory into `/usr/local`

In otherword, in `/usr/local` are

- /usr/local/SoundShow/
- /usr/local/SoundShow-soundfiles
- /usr/local/SoundShow.ssp

This is the contens of the desktop file to launch it.

```
[Desktop Entry]
Version=1.0
Type=Application
Name=SoundShow
Comment=Masonic Lodge Music
Exec=/usr/local/SoundShow/SoundShow.x86_64
Icon=/usr/local/share/SoundShow/SoundShow_Data/Resources/UnityPlayer.png
Terminal=false
```

# Make a bootable image

Download the [Alpine minirootfs tarball](https://wiki.alpinelinux.org/wiki/Installation).

Install Gnome (I chose Wayland windowing)
