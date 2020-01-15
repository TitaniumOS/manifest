![TitaniumOS](https://github.com/Titanium-OS/manifest/raw/ten/TitaniumOS-banner.png)

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

    repo init -u git://github.com/TitaniumOS/manifest -b ten
    

Then to sync up:
----------------

    repo sync -j8 --force-sync -c --no-clone-bundle --no-tags --optimized-fetch --prune

Build command is:
----------------
    . build/envsetup.sh
    lunch titanium_($device)-userdebug
    make titanium

## Report build issues
- You can reach us via [Telegram](https://t.me/TitaniumOS_Chat)

