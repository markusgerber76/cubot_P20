# cubot_P20


Cheap and cheerful


## Specs

See here for [specifications](https://www.gizmochina.com/product/cubot-p20/).


## Treble

ships with Android oreo

<p align="center">
<img src="https://raw.githubusercontent.com/voltcraft1/cubot_P20/master/cubot_treble.png"
  alt="Treble info"
  width="600" >
</p>


## Download GSI treble

Download arm64 (not binder) from 

https://github.com/phhusson/treble_experimentations/wiki



https://github.com/eremitein/treble-patches/wiki/CAOS-Project

https://forum.xda-developers.com/project-treble/trebleenabled-device-development/gsi-lineageos-17-0-gsi-archs-t4004673

Uncompress image

```
xz -d lineage-17.1-20200808-UNOFFICIAL-treble_arm64_avN.img.xz
```

## Unlock bootloader



Connect phone.



```

$ adb reboot bootloader
$ fastboot devices

$ fastboot flashing unlock

```

Accept using volume-UP on device. Device reboots. Then say OK. Enable adb then reboot to bootloader


## Installing GSI treble


```
fastboot erase system
fastboot flash system  lineage-17.1-20200808-UNOFFICIAL-treble_arm64_avN.img
```

## Very likely the complete 64GB space is NOT recognised.

* Reboot to recovery using 
```
adb reboot recovery
```
or
```
Shutdown phone. Press and hold Volume UP and power

```

In the recovery menu:

* Wipe cache partition
* Wipe data/factory reset
* Restart phone


## Plenty of free space


<p align="center">
<img src="https://raw.githubusercontent.com/voltcraft1/cubot_P20/master/freespaceFiles.png"
  alt="Treble info"
  width="400" >
</p>


<p align="center">
<img src="https://raw.githubusercontent.com/voltcraft1/cubot_P20/master/storage.png"
  alt="Treble info"
  width="400" >
</p>

