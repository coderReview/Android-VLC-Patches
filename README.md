Android-VLC-Patches
===================

Follow the steps in https://wiki.videolan.org/AndroidCompile to download and compile VLC for Androd.

After the compilation is finished apply the patches inside android-vlc folder:

> git apply --verbose $PATH_TO_REPOSITORY/android-vlc/0001-Support-multiple-video-player-instances.patch

Change to vlc folder and apply patch:

> cd vlc/
> git apply --verbose $PATH_TO_REPOSITORY/vlc/0001-Support-for-multiple-video-instances.patch
> cd ../

Recompile the code:
> ./compile.sh --build

