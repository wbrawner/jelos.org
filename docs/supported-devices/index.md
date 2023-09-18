<!---
icon: material/monitor
--->

# Supported Devices

JELOS supports a variety of ARM and Intel/AMD based devices<sup>1</sup>.  

| Manufacturer | Device | CPU / Architecture | Kernel | GL driver | Interface |
|--|--|--|--|--|--|
|Anbernic| RG351P/M | Rockchip RK3326 (ARM) | Mainline Linux | Panfrost | Weston + EmulationStation|
|Anbernic| RG353P<sup>2</sup> | Rockchip RK3566 (ARM) | Rockchip BSP 4.19 | Mali | KMS/DRM + EmulationStation|
|Anbernic| RG353M<sup>2</sup> | Rockchip RK3566 (ARM) | Rockchip BSP 4.19 | Mali | KMS/DRM + EmulationStation|
|Anbernic| RG353V<sup>2</sup> | Rockchip RK3566 (ARM) | Rockchip BSP 4.19 | Mali | KMS/DRM + EmulationStation|
|Anbernic| RG353VS<sup>2</sup> | Rockchip RK3566 (ARM) | Rockchip BSP 4.19 | Mali | KMS/DRM + EmulationStation|
|Anbernic| RG503 | Rockchip RK3566 (ARM) | Rockchip BSP 4.19 | Mali | KMS/DRM + EmulationStation|
|Anbernic| RG552 | Rockchip RK3399 (ARM) | Mainline Linux | Panfrost | Weston + EmulationStation|
|Anbernic|Win600|AMD Athlon Silver 3050e (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|Atari|VCS|AMD Ryzen R1606G (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|AOKZOE | A1 Pro | AMD 7840u (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|AYANEO<sup>3</sup>|Air / Air Pro|Amd Ryzen 5 5560U / AMD Ryzen 7 5825U (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|AYANEO<sup>3</sup>|Air Plus|Amd Ryzen 7 6800U / (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|AYANEO<sup>3</sup>|AYANEO 2|Amd Ryzen 7 6800U / (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|Ayn|Loki Zero|AMD Athlon Silver 3050e (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|Ayn|Max|Amd Ryzen 7 6800U / (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|GPD|Win 4|Amd Ryzen 7 6800U / (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|GPD|Win Max 2 (2022)|Amd Ryzen 7 6800U / (x86_64)|Mainline Linux|Radeonsi|Weston + EmulationStation|
|Hardkernel| Odroid Go Advance | Rockchip RK3326 (ARM) | Mainline Linux | Panfrost | Weston + EmulationStation|
|Hardkernel| Odroid Go Super | Rockchip RK3326 (ARM) | Mainline Linux | Panfrost | Weston + EmulationStation|
|Hardkernel|Odroid Go Ultra|Amlogic S922X / Mali G52 M6 (ARMv8-A)|Mainline Linux|Mali|Weston + EmulationStation|
|Indiedroid|Nova|Rockchip RK3588S / Mali G610 (ARMv8-A)|Rockchip 5.10 BSP Linux|Panfrost|Weston + EmulationStation|
|Orange Pi|Orange Pi 5|Rockchip RK3588S / Mali G610 (ARMv8-A)|Rockchip 5.10 BSP Linux|Panfrost|Weston + EmulationStation|
|Powkiddy|RGB10 Max 3 Pro|Amlogic A311D / Mali G52 M4 (ARMv8-A)|Mainline Linux|Mali|Weston + EmulationStation|
|Powkiddy| RGB30 | Rockchip RK3566 (ARM) | Rockchip BSP 4.19 | Mali | KMS/DRM + EmulationStation |
|Powkiddy| RK2023 | Rockchip RK3566 (ARM) | Rockchip BSP 4.19 | Mali | KMS/DRM + EmulationStation |
|Powkiddy| x55 | Rockchip RK3566 (ARM) | Rockchip BSP 4.19 | Mali | KMS/DRM + EmulationStation |

> <sup>1</sup> While not technically supported, JELOS is known to work well on a variety of generic x86_64 devices including gaming PCs, mini PCs, and laptop computers.

> <sup>2</sup> Anbernic RG353P/M/V/VS devices with both v1 and v2 displays are supported.  RG353PS will not be supported.

> <sup>3</sup> To boot JELOS on Ayaneo devices, hold LC and volume up and press the power button, continue holding "LC" and volume up until the Ayaneo logo appears.  Select the storage device with JELOS from the boot menu using the Ayaneo button, and then press volume up to boot the distribution.