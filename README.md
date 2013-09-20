INTRO
=====

Andoroid Ice Cold Project (AICP) is an AOKP enhanced rom.
Big credits go to AOKP team and their contributors!!!
We'll try to follow AOKP's guidelines and add a little special from our side.
Visit http://gerrit.zips.co for code review




INITIALIZING REPOSITORY
=======================

Init core trees without any device/kernel/vendor :

    $ repo init -u https://github.com/AICP/platform_manifest.git -b jb-mr2

Init repo with all devices, kernels and vendors supported by AICP :

    $ repo init -u https://github.com/AICP/platform_manifest.git -b jb-mr2 -g all,kernel,device,vendor

Init repo only for a particular device :

    $ repo init -u https://github.com/AICP/platform_manifest.git -b jb-mr2 -g all,-notdefault,<devicename>,<vendorname>

for example, to init only trees needed to build m7ul :

    $ repo init -u https://github.com/AICP/platform_manifest.git -b jb-mr2 -g all,-notdefault,m7,htc

Init repo for multiple devices :

    $ repo init -u https://github.com/AICP/platform_manifest.git -b jb-mr2 -g all,-notdefault,<devicename1>,<devicename2>,<devicename3>,<vendorname1>,<vendorname2>,<vendorname3>

for example, to init trees needed to build m7ul and flo :

    $ repo init -u https://github.com/AICP/platform_manifest.git -b jb-mr2 -g all,-notdefault,m7ul,flo,lge,asus


sync repo :

    $ repo sync
