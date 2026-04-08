# 联想 拯救者 Y9000X 2021 黑苹果(Lenovo Legion S7 15IMH5) Hackintosh
</br>
</br>
机型看官网(本机配置如下)：
https://psref.lenovo.com/WDProduct/Legion/Lenovo_Legion_S7_15IMH5
</br>
</br>
CPU：Intel Core i7-10870H Comet Lake</br>
核显：Intel UHD Graphics 630 </br>
独显：NVIDIA GeForce GTX 1650 Ti </br>
主板：Intel HM470 chipset </br>
内存：8GB + 16GB DDR4-3200 </br>
硬盘：2TB SSD PM981A NVMe </br>
声卡：Realtek ALC3306 </br>
网卡：Intel Wi-Fi 6 AX201 + Bluetooth 5.1</br>
屏幕：BOE 15.6" FHD (1920x1080) IPS 144Hz</br>
接口：USB 3.2 Gen 2 / Thunderbolt 3</br>
读卡器：4-in-1 card reader (SD, SDHC, SDXC, MMC)</br>
</br>
</br>
# 黑苹果前期工作：
本机只需要进BIOS，关闭secure boot，config.plist的三码改一下。</br>
</br>
最新进展：</br>
1.因为PM981A，只能用SSDT-DNVMe.aml屏蔽掉，目前是安装在USB固态硬盘的，还没有添加NVME驱动，后面打算买个SN730加装</br>
2.装的是Sequoia 15.7.5版本，基本驱动已经完成，能正常开机，指纹没用，扬声器没修复，只能戴耳机，背光亮度不能调，睡眠那些也没做</br>
</br>
Y9000X 2021笔记本其实一直用Windows 10几年了，最近想玩一下黑苹果，很遗憾，搜索整个网络都没有同机型的EFI可用，只好从近似机型去找，走了不少弯路，所以才跑Github来建档分享一下，顺便找找同机型的用户，你们在哪里？</br>
</br>
</br>
没有用VPN，国内访问github时好时坏的...</br>
</br>
</br>
2026-4-8 </br>
在Github建档，OC版本1.0.7，Clover版本r5172，主要是想记录下过程，目前还在摸索阶段，欢迎同机型的探讨！</br>
</br>

# 主要EFI文档来源：</br>
https://olarila.com/files      这个论坛提供的EFI真的非常齐全，通用性强 </br>
https://github.com/gclm/Hackintosh-LEGION-Y7000P-I7-9750H </br>
其实找了很多十代平台的EFI，包括其他品牌同款CPU i7-10875H的都不能启动，找到这里的EFI文件是唯一的一个能启动的！但定制的东西太多吧，又是9代平台的，OC的EFI在本机不能启动，试了一下clover-5144的能启动Sonoma，这才开始了从clover的修改之旅！学了一些配置知识后，才跟进OC的</br>
</br>
</br>
工具、驱动来源：</br>
https://github.com/acidanthera </br>
https://github.com/CloverHackyColor </br>
</br>
https://github.com/benbaker76/Hackintool </br>
https://mackie100projects.altervista.org </br>
https://github.com/btwise/OpCore-Simplify </br>
</br>
https://github.com/USBToolBox</br>
https://github.com/CrisHotpatch/USBInjectAll </br>
https://github.com/VoodooI2C/VoodooI2C </br>
https://github.com/OpenIntelWireless </br>
https://github.com/1Revenger1/ECEnabler </br>
</br>
</br>
非常感谢他们的分享！</br>
