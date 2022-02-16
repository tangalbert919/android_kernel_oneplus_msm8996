4.4 kernel for OnePlus 3/3T
==========

Right now it boots to LineageOS 18.1 (maybe)

## What works (outdated)

* Display
* Sound
* Camera
* Touchscreen (but keypad fw update leads to a kernel panic)
* NFC
* WiFi/BT/RIL
* Vibrator
* Sensors

## What doesn't work (outdated)

* USB
* The entire power stack (including battery and dash charger)
* Other random unnoticed stuff

## Future work

* Rewrite part of the power stack to fix it. The power supply framework was refactored a lot from 3.18 to 4.4. MSM8996 uses QPNP SMB Charger while MSM8998 uses SMB2 Battery Charger so we can't kang from OP5/5T despite they're from the same OEM.
* Backport eBPF so this kernel can also boot on LineageOS 19.0.
* Merge latest patches from Linux kernel 4.4.302.
* This is dianlujitao's unfinished port rebased on an updated 4.4 kernel from CodeAurora. It is very likely that this port will also be unfinished, as I am developing this in my spare time.

## Contribute

* Contributions to are welcomed and appreciated. Feel free to send a pull request containing **bug fixes** towards the port. Warning fixes, security patches, features and other rices will be **ignored**.
