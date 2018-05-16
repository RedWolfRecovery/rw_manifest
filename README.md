## Getting Started ##
---------------

To get started with building Red Wolf Recovery, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

To initialize your local repository using the minimal-manifest-twrp omni trees to build Red Wolf Recovery, use a command like this:

    repo init -u git://github.com/RedWolfRecovery/rw_manifest.git -b rw-n
    
To initialize a shallow clone, which will save even more space, use a command like this:

    repo init --depth=1 -u git://github.com/RedWolfRecovery/rw_manifest.git -b rw-n

Then to sync up:

    repo sync

Then to build:

     cd <source-dir>; . build/envsetup.sh; lunch omni_<device>-eng; mka recoveryimage
