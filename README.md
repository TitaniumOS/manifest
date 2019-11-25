# TitaniumOS #

Credits:
=======
 * [**AOSP**](https://android.googlesource.com)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**AOSiP**](https://github.com/AOSiP)
 * [**PixelExperience**](https://github.com/PixelExperience)

-----------------------------------------------------------------------------
Getting Started:
================

Create titanium folder:
----------------------

    mkdir ~/titanium
    cd ~/titanium
    

GIT config (nickname, e-mail):
-----------------------------

    git config --global user.email "mail@domain.com"
    git config --global user.name "login"
    

To initialize your local repository use:
---------------------------------------

    repo init -u https://github.com/Titanium-OS.git -b ten
    

Then to sync up:
----------------

    repo sync -j 16

Build command is:
----------------
    export JACK_SERVER_VM_ARGUMENTS="-Dfile.encoding=UTF-8 -XX:+TieredCompilation -Xmx4000m"
    . build/envsetup.sh
    lunch titanium_raphael-userdebug or lunch titanium_raphael-userdebug
    make -j 7 otapackage

## Report build issues
- You can reach us via [Telegram](#)

