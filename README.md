Local manifest to build CyanogenMod 12.1 UNOFFICIAL for [Alcatel Pop3 (5) 5065D](https://4pda.ru/forum/index.php?showtopic=704708)

How to download:
-------------

Initialize repo:

    repo init -u git://github.com/LineageOS/android.git -b cm-12.1
    curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.githubusercontent.com/zombah/android_local_manifest_alcatel_pop35/cm-12.1/local_manifest.xml
    repo sync


How to compile:
------------

    source ./build/envsetup.sh
    lunch cm_pop35-userdebug
    make otapackage
