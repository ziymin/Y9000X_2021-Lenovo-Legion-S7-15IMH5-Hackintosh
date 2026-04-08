# Lenovo LEGION Y9000X 2021 (Lenovo Legion S7 15IMH5)  Hackintosh

</br>
</br>
机型配置看官网(本机如下)：
https://psref.lenovo.com/WDProduct/Legion/Lenovo_Legion_S7_15IMH5
</br>
</br>
Intel Core i7-10870H (8C / 16T, 2.2 / 5.0GHz, 16MB) </br>
NVIDIA GeForce GTX 1650 Ti 4GB GDDR6 </br>
Intel UHD Graphics 630 </br>
Intel HM470 chipset </br>
8GB Soldered DDR4-3200 + 16GB SO-DIMM DDR4-3200 </br>
2TB SSD NVMe PM981A </br>
Realtek ALC3306 </br>
Stereo speakers, 2W x2, Dolby Atmos for gaming </br>
4-in-1 card reader (SD, SDHC, SDXC, MMC)</br>
BOE 15.6" FHD (1920x1080) IPS 300nits 144Hz</br>
Intel Wi-Fi 6 AX201 + Bluetooth 5.1</br>
USB 3.2 Gen 2 / Thunderbolt™ 3</br>
</br>
</br>
最新进展：</br>
1.因为PM981A黑不了，目前是安装在USB固态硬盘的，还没有添加NVME驱动，后面打算买个SN730</br>
2.装的是Sequoia 15.7.5版本，基本驱动已经完成，正常开机使用，外放没驱动，只能戴耳机，背光亮度不能调，睡眠那些也没做</br>
</br>
没有用VPN，国内访问github时好时坏的...</br>
</br>
</br>
Y9000X 2021笔记本其实一直用Windows几年了，最近想玩一下黑苹果，很遗憾，搜索整个网络都没有同机型的EFI可用，</br>
只好从近似机型去找，走了不少弯路，所以才跑Github来建档分享一下，顺便找找同机型的用户，你们在哪里？</br>
</br>
</br>
2026-4-8 </br>
在Github建档，主要是想记录下过程，目前还在摸索阶段，欢迎同机型的讨论！</br>
</br>

# 主要EFI文档来源：</br>
https://olarila.com/files      这个论坛提供的EFI真的非常齐全，通用性强 </br>
https://github.com/gclm/Hackintosh-LEGION-Y7000P-I7-9750H </br>
其实找了很多十代机型的EFI，包括其他品牌同款CPU i7-10870H的都不能启动，找到这里的EFI文件是唯一的一个能启动的！<br>
但定制的东西太多吧，又是9代平台的，OC的EFI在本机不能启动，试了一下clover的能启动Sonoma，这才开始了修改之旅！</br>
</br>
</br>
工具、驱动来源：</br>
https://github.com/acidanthera </br>
https://github.com/CloverHackyColor </br>
</br>
https://github.com/benbaker76/Hackintool </br>
https://mackie100projects.altervista.org </br>
https://github.com/USBToolBox</br>
</br>
https://github.com/VoodooI2C/VoodooI2C </br>
https://github.com/CrisHotpatch/USBInjectAll </br>
https://github.com/OpenIntelWireless </br>
https://github.com/1Revenger1/ECEnabler </br>
</br>
</br>
非常感谢他们的分享！</br>
</br>
</br>
