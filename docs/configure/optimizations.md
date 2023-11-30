# :material-battery-plus: Optimizations

JELOS provides a variety of settings that allow you to optimize for battery life or performance globally, on a per system and per game basis.  For emulating 6th generation and later systems, we recommend installing JELOS on internal storage if available to reduce IO bottlenecks reading and writing shader cache.

## Optimizing For Performance

Optimizing for performance will have significant impact on battery life, however it will also provide the best experience for more demanding emulators.

### Recommended Global Settings

#### AMD / Intel based devices

|Enabled CPU Threads|CPU Scheduler|Energy Performance Preference|GPU Performance Profile|Enhanced Power Saving|Cooling Profile|WIFI Power Saving|
|----|----|----|----|----|----|----|
|All|Schedutil|Balanced Performance|Balanced|Off|Moderate<sup>1</sup> or Auto|Off|

> Note: The JELOS team DOES NOT recommend the "BEST PERFORMANCE" GPU profile on AMD devices as it sets the profile_peak GPU profile which can lead to poor performance and kernel panics, use "BALANCED" instead.

##### GLMark
|DEVICE @ TDP|4w|6w|9w|15w|18w|24w|28w|
|----|----|----|----|----|----|----|----|
|Loki Zero|515|1303|1943|3195|3466|3615|**3618**|
|Loki Max|2082|3068|4910|7266|8600|9990|**10319**|
|AYANEO Air Plus|854|2051|4192|5946|7340|9325|**9674**|
|Atari VCS|534|565|1055|1342|1376|**1378**|1376|

##### 7z
|DEVICE @ TDP|4w|6w|9w|15w|18w|24w|28w|
|----|----|----|----|----|----|----|----|
|Loki Zero|3370|5304|7397|8441|**8514**|8493|8441|
|Loki Max|12129|19530|28391|42809|46432|51183|**53276**|
|AYANEO Air Plus|6323|11394|22519|39682|43529|**47904**|47562|
|Atari VCS|5015|6172|9027|**9726**|9239|9233|9257|

#### ARM based devices

|Enabled CPU Threads|CPU Scheduler|GPU Performance Profile|Enhanced Power Saving|Cooling Profile|WIFI Power Saving|
|----|----|----|----|----|----|
|All|Performance|Best Performance|Off|Moderate<sup>1</sup> or Auto|Off|

> Note: It's recommended to reboot the device after disabling Enhanced Power Saving.

## Optimizing For Battery Life

JELOS includes an `Enhanced Power Saving` mode which is available in the `System Settings` menu.  This option provides a variety of sub options that when enabled tune your device for optimal battery life without immediately sacrificing performance.

|Feature|Function|May Affect Stability|
|----|----|----|
|CPU Power Saving|Tunes the CPU/SoC to preference battery life over performance.|No|
|Audio Power Saving|Enables the audio device to operate in a low power mode.|No|
|PCIE Active State Power Management|Forces a low power state for PCI and PCIe connections.|Yes|
|Enable Wake Events|Enables PCI wakeup signalling to allow devices to enter low power states.|Yes|
|Runtime Power Management|Enables USB idle power management, and configures usb devices to autosuspend.|Yes|

### Recommended Settings

Enable Enhanced Power Saving, and enable all options.  If the device has undesired behavior, disable the options that may effect stability and reboot the device.

#### AMD / Intel based devices
|Enabled CPU Threads|CPU Scheduler|Energy Performance Preference|GPU Performance Profile|Enhanced Power Saving|Cooling Profile|WIFI Power Saving|
|----|----|----|----|----|----|----|
|4|Powersave|Power Saving|Battery Focus|On|Quiet<sup>1</sup>|On|

> JELOS recommends setting the minimum TDP that offers full performance for your game or system.

##### GLMark
|DEVICE @ TDP|4w|6w|9w|15w|18w|24w|28w|
|----|----|----|----|----|----|----|----|
|Loki Zero|544|1130|1313|1385|1378|1392|1397|
|Loki Max|1968|2869|4660|7042|8243|9442|9804|
|AYANEO Air Plus|744|2103|3971|6086|7193|8908|9377|
|Atari VCS|305|332|332|332|333|333|332|

##### 7z
|DEVICE @ TDP|4w|6w|9w|15w|18w|24w|28w|
|----|----|----|----|----|----|----|----|
|Loki Zero|2980|2986|3006|2992|2992|2993|2978|
|Loki Max|6931|11247|14003|15941|16114|16758|16792|
|AYANEO Air Plus|5731|8291|13139|15638|16205|16065|16001|
|Atari VCS|2464|4513|4530|4524|4531|4529|4549|

#### ARM based devices

|Enabled CPU Threads|CPU Scheduler|GPU Performance Profile|Enhanced Power Saving|Cooling Profile|WIFI Power Saving|
|----|----|----|----|----|----|
|4|Powersave|Battery Focus|On|Quiet<sup>1</sup>|On|

## Recommended Settings Per System

### AMD / Intel
As performance varies across supported devices, there are no specific recommendations.  Explore various settings to find the best configuration per system/game for your device.

### ARM Devices
|Manufacturer|System|Enabled CPU Threads|Cooling Profile|Scaling Governor|Enhanced Power Saving|WIFI Power Saving|
|----|----|----|----|----|----|----|
|Nintendo|64|All|Moderate<sup>1</sup>|Performance|On|On|
|Nintendo|GameCube, Wii|All|Moderate<sup>1</sup>|Performance|On|On|
|Sega|Saturn, Dreamcast|All|Moderate<sup>1</sup>|Performance|On|On|
|Sony|PSP|All|Moderate<sup>1</sup>|Performance|On|On|

> <sup>1</sup> Only available if the feature is supported on your device.
