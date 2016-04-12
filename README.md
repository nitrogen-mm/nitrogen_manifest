Nitrogen OS Manifest
===================

Create dirs, and install soft, libs
-----------------------------------

    sudo su
    apt-get install bison build-essential curl flex lib32ncurses5-dev lib32readline-gplv2-dev lib32z1-dev libesd0-dev libncurses5-dev libsdl1.2-dev libwxgtk2.8-dev libxml2 libxml2-utils lzop openjdk-7-jdk openjdk-7-jre pngcrush schedtool squashfs-tools xsltproc zip zlib1g-dev git-core make phablet-tools gperf
    exit
    
    
Install repo
------------

    mkdir ~/bin
    PATH=~/bin:$PATH
    cd ~/bin
    curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
    chmod a+x ~/bin/repo
    

Create nitrogen folder
----------------------

    mkdir ~/nitrogen
    cd ~/nitrogen
    

GIT config (nickname, e-mail)
-----------------------------

    git config --global user.email "mail@domain.com"
    git config --global user.name "login"
    

To initialize your local repository use
---------------------------------------

    repo init -u https://github.com/nitrogen-project/nitrogen_manifest.git -b mm6.0-all
    

Then to sync up:
----------------

    repo sync --force-sync

Build command is
----------------

    cd ~/nitrogen
    . builder

Supported Devices
-----------------

LG Optimus G (geehrc)

LG Optimus G (geeb)

LG Nexus 4 (mako)

LG Nexus 5 (hammerhead)

Android One (Sprout 4)

Android One (Sprout 8)
