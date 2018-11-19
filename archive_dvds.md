# How to rip DVDs with Handbrake

## Install Handbrake
*DISCLAIMER: This information is to be used to archive DVDs that you own.*

* Official [Source](https://github.com/HandBrake/HandBrake)
* [Download](https://handbrake.fr/downloads.php) handbrake for your specific host -

## Install libdvdcss
* Most purchased DVDs are protected.  To rip protected DVDs install libdvdcss - [https://www.videolan.org/developers/libdvdcss.html](https://www.videolan.org/developers/libdvdcss.html)
* Mac install of libdvdcss via brew
```
command + space
terminal
sudo xcode-select --install
sudo xcodebuild -license accept
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install libdvdcss
```

## Ripping DVDs in Hanbrake
* Open Source -> select an ISO file or a DVD drive
* Audio -> add language tracks
* Subtitles -> add subtitle tracks
* Format -> MP4 Format (this format is more portable for android and standard players)
* Save As -> Set your name (mp4 format saves as .m4v)
* Start or Add to queue

## How to watch .m4v
* VLC player is a very good media player.  It supports streaming (i.e. DLNA)
* Install VLC player - https://www.videolan.org/vlc/download-macosx.html or download it via the app store on iOS or android
* Other players work such as quicktime for iOS and macOS or video.  I use VLC on my android devices

## Setup a streaming server
* Buy a NAS - i.e. Buffalo NAS LInkStation 400 devices - https://www.buffalotech.com/products/category/network-attached-storage-nas.  These NAS devices support a variety of features like DNLA to stream videos, backup features for MAC and windows, SAMBA, NFS, etc.
* The NAS can be skipped.  I use it for flexibility and run my own personal cloud storage instead of relying on iCloud, Google Drive, MS OneDrive, Dropbox, etc.  If skipping the NAS, the PLEX server MUST have a large hard drive.  If using a NAS, SAMBA or NFS mount the drive from the PLEX server.  If a NAS is not used, the PLEX server can use its local drives.
* Setup a PLEX server.  My setup uses a $35 rasberi pi.  The main thing is to reduce WIFI usage by connecting the PLEX server host and the NAS to a WIFI router directly via an ethernet cable.
* Install PLEX clients on devices.
