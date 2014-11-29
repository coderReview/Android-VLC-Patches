Android-VLC-Patches
===================

Follow the steps in [AndroidCompile](https://wiki.videolan.org/AndroidCompile) to download and compile VLC for Androd.
To use the commit hash shown below, after cloning the repository do:

> git checkout 7a5c3cda60784b10510f3394c2f1b70e53292b91

After the compilation is finished apply the patches inside android-vlc folder:

> git apply --verbose $PATH_TO_REPOSITORY/android-vlc/0001-Fix-package-name-for-expandMedia-and-loadPlaylist-na.patch

> git apply --verbose $PATH_TO_REPOSITORY/android-vlc/0001-Add-support-for-multiple-video-instances.patch

Change to vlc folder and apply patch:

> cd vlc/

Run:

> git pull origin master

> git checkout f1403d277547f10ba2d14d3bcbf86251c6c5f759

> git apply --verbose $PATH_TO_REPOSITORY/vlc/0001-Fix-issue-with-jni_ConfigureSurface-return-value.patch

> git apply --verbose $PATH_TO_REPOSITORY/vlc/0001-Add-support-for-multiple-video-instances.patch 

> cd ../

Recompile the code:
> ./compile.sh --build

Example App:
------------

For an example application please check https://github.com/Ambigioz/multiplevlc.

Note:
=====

The patches are based on android vlc commit hash 7a5c3cda60784b10510f3394c2f1b70e53292b91.

