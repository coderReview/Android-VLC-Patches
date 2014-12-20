Android-VLC-Patches
===================

Follow the steps in [AndroidCompile](https://wiki.videolan.org/AndroidCompile) to download and compile VLC for Androd.
To use the commit hash shown below, after cloning the repository do:

> git checkout 8b51735dab3c473f9697aa14c0b4b800fc217987

After the compilation is finished apply the patches inside android-vlc folder using "git apply" command.

Change to vlc folder and apply patch:

> cd vlc/

Run:

> git pull origin master

> git checkout 5967150642d875f12aa69ecc853e935fc593077a

Apply patches using "git apply" command.

> cd ../

Recompile the code:
> ./compile.sh --build

Example App:
------------

For an example application please check https://github.com/Ambigioz/multiplevlc.

Compiled libraries:
------------------

Compiled libraries and Java source code can be found in the sdk/ folder.

Note:
=====

The patches are based on android vlc commit hash 8b51735dab3c473f9697aa14c0b4b800fc217987.

