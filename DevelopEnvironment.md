How to Start iOS develop on Linux?
===================================

Here, we just use archlinux.

1. install llvm and clang

    $ pacman -S llvm clang

2. install ios-toolchain

    $ yaourt ios-toolchain

3. install ios-sdk, here we install ios sdk 6

    $ yaourt ios-sdk6

4. install utils.

    $ yaourt iphonesdk-utils

5. start an example project

    $ ios-createProject 
    iPhone Project Createor
    ---------------------------

    [0.] Application
    [1.] Command line utility
    [2.] Dynamic Framework
    [3.] Dynamic Library
    [4.] Notification Center widget
    [5.] Static Framework
    [6.] Static Library
    [7.] Example Player
    [8.] Example UICatalog
    Choose a Template:8
    Project Name:Controls
    ---------------------------

    Project Controls generated in ./Controls folder.

6. build the example project.

    $ cd Controls/
    $ make

How to install the app into your phone?
========================================

Note: your phone must be jailbreaked.

1. build xxx.app directory

    $ make dist

2. edit Makefile, setup IPHONE_IP for iphone ip.

3. install app

    $ make install
