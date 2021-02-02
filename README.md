![TitaniumOS](https://github.com/TitaniumOS/manifest/raw/eleven/snippets/TitaniumOS-banner.png)

# TitaniumOS #

Credits:
=======
 * [**AOSP**](https://android.googlesource.com)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**Evolution-X**](https://github.com/Evolution-X)
 * [**Havoc-OS**](https://github.com/Havoc-OS)
 * [**Project-Xtended**](https://github.com/Project-Xtended)
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

    repo init -u git://github.com/TitaniumOS/manifest -b eleven
    

Then to sync up:
----------------

    repo sync -j$(nproc --all) --no-tags --no-clone-bundle

Build command is:
----------------
    . build/envsetup.sh
    lunch titanium_($device)-userdebug
    make titanium -j$(nproc --all)
    
Inheriting Gapps in build:
-------------------------
• To include Gapps in your builds, execute:

     export WITH_GMS=true
     
• For including stock gapps packages, execute:

     export TARGET_INCLUDE_STOCK_GAPPS=true
     
• For including pixel live wallpapers, execute:

     export TARGET_INCLUDE_LIVE_WALLPAPERS=true

• Also in addition to this...
If any apps you would like to get it removed in gapps package, just add

     For e.g:

     REMOVE_GAPPS_PACKAGES += \
              Chrome \
              CalculatorGoogle
## Report build issues
- You can reach us via [Telegram](https://t.me/TitaniumOS_Chat)
