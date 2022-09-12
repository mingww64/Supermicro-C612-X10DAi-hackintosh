

![interview](https://github.com/wmyfelix/X10DAi-hackintosh/blob/main/interview.png?raw=true)
![](https://github.com/wmyfelix/Supermicro-C612-X10DAi-hackintosh/blob/main/Screenshot_20220912_170714.png?raw=true)
# Run macOS on the Supermicro X10DAi 
|Support macOS ver.|11.2|
|:-|-|
|Bootloader|OpenCore 0.67 DBG|
|CPU Platform|Haswell-EP(E5v3)

|System Configuraion||notes|
|:-|:-:|:-:|
|CPU|Xeon E5 2695v3 ES x2|XCPM works, not sure if it schedule correctly|
|Graphics|Radeon Pro Duo Fiji |Mod to add GoP support| 
|BIOS|X10DAi9.C16|Mod to unblock cfg lock and add nvme support|
|Sounds|Creative usb external card|Use soundsource to adjust volume|
|Keyboard|ikbc F87|Update [firmware](https://share.weiyun.com/riG5w1hT) to fix the misfunctioning typing|
|Disk|WD sn720 *4 |PCIe Extension Card|added deviceproperties and set to "bulit-in"|
|Monitor|3840x2160 27' |DP|
* __issues__ 
  * __Sleep__
  * __~~Unpredictable window freeze~~:__ `$ defaults write com.apple.coremedia hardwareVideoDecoder disable`
  * __Onboard-audio not test but should work__ *//my alc888 is broken*
  * _Some logs uploaded,feel free to contact me._  
*** 
__As for the Broadwell(E5-26XXV4) CPU, it requires to change some stuffs like the Fake CPU ID, see [dortania guide](https://dortania.github.io/OpenCore-Install-Guide/config-HEDT/broadwell-e.html#acpi/)__  


