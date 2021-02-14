# X10DAi hackintosh
## Supermicro X10DAi running macOS
|current version|11.2|
|:-|-|
|bootloader|OpenCore 0.66 DBG|

|system-configs||notes|
|:-|:-:|
|CPU|Xeon E5 2695v3 ES x2|xcpm work,not sure if cpu Scheduling correct|
|Graphics|Radeon Pro Duo Fiji |modding vbios to add GoP support,switch legacy to EFI corresponding to PCIE slot in bios PCIE configuration| 
|Disk|WD sn720 x4 |via PCIE|not sure if nvmefix is a must|
|Monitor|3840x2160 27' |connect via DP|
* __issues__ 
  * __Sleep__
  * __Unpredictable window frezze,force reboot needs__
  * __Onboard-audio not test but should work__ *//my alc888 is broken*
  * _Some logs uploaded,if you need more detail feel free to contact me._
**for v4 cpu user,needs to change some stuffs like fake cpu id,more info: https://dortania.github.io/OpenCore-Install-Guide/ **
