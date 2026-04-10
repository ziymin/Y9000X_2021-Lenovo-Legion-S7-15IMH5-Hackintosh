# 联想 拯救者 Y9000X 2021 黑苹果EFI - Lenovo Legion S7 15IMH5 Hackintosh
</br>
https://psref.lenovo.com/WDProduct/Legion/Lenovo_Legion_S7_15IMH5
</br>
</br>
国外型号：Lenovo Legion Y740S-15IMH  这个好合适黑苹果啊
</br>
https://psref.lenovo.com/WDProduct/Legion/Lenovo_Legion_Y740S15IMH
</br>
</br>
本机型配置如下：
</br>
CPU：Intel Core i7-10870H Comet Lake </br>
核显：Intel UHD Graphics 630 </br>
独显：NVIDIA GeForce GTX 1650 Ti </br>
主板：Intel HM470 chipset </br>
内存：8GB + 16GB DDR4-3200 </br>
硬盘：2TB SSD PM981A NVMe </br>
声卡：Realtek ALC3306 </br>
网卡：Intel Wi-Fi 6 AX201 + Bluetooth 5.1 </br>
屏幕：BOE 15.6" FHD (1920x1080) IPS 144Hz </br>
接口：USB 3.2 Gen 2 / Thunderbolt 3 </br>
读卡器：4-in-1 card reader (SD, SDHC, SDXC, MMC) </br>
</br>
</br>
本EFI使用说明：</br>
1.进入BIOS，关闭secure boot；下载好EFI文件夹内有ZIP文件的先解压，config.plist三码改一下
</br>
2.如果你的固态硬盘支持黑苹果，需要先添加NVMe补丁识别
</br>
3.建议用USBToolBox专门定制一下USB端口映射，生成新的UTBMap.kext替换掉，很多问题都好解决了。这里https://github.com/USBToolBox/tool 下载Windows版的。USBToolBox+UTBMap方案或者USBInjectAll方案，二选一即可，但在Clove中可能其他地方没配置好，不能用USBInjectAll
</br>
4.上网需要安装一个HeliPort的APP，这里https://github.com/OpenIntelWireless/HeliPort
</br>
</br>
PS：Y9000X 2021笔记本其实一直用Windows 10几年了，最近想玩一下黑苹果，很遗憾，搜索整个网络都没有同机型的EFI可用，只好从近似机型去找，很奇怪，为什么没有十代CPU的拯救者用户吗？走了不少弯路，所以才跑Github来建档分享一下，顺便找找同机型的用户，你们在哪里？
</br>
</br>
说一下Clover和OC，个人其实更喜欢Clover的，简单易用，兼容性强，OC稍微有点硬件配置问题，就会完全崩溃，搞不懂开发人员为何将重点放到了OC上~~~
</br>
</br>
没有用VPN，国内访问github时好时坏的...</br>
</br>
</br>
最新进展：
</br>
因为PM981A，只好用SSDT-DNVMe.aml屏蔽掉，我目前是安装在USB固态硬盘测试的，还没有添加NVMe驱动。系统版本是Sequoia15.7.5，基本驱动已经完成，大部分功能都可以正常使用，指纹用不了，扬声器没修复，只能戴耳机，背光亮度不能调，睡眠那些也没完善
</br>
</br>
2026-4-10 
</br>
https://github.com/Cuveanst/Y9000X-2020-Sequoia-15.7.4-EFI 
</br>
想修复扬声器来的，结果能找到最接近的解决方案就是这个了，但是安装后并不生效，除非在这个基础上再改改，本人不会编程，所以只能等待高人解决。其他一些能做的都做了，深感能力有限啊，估计不会有什么新进展了
</br>
</br>
2026-4-8 </br>
在Github建档，OC版本1.0.7，Clover版本r5172，主要是想记录下过程，目前还在摸索阶段，欢迎同机型的爱好者一起探讨完善！
</br>
</br>

# 主要EFI文档来源：</br>
https://olarila.com/files   这个论坛提供的EFI真的非常齐全，通用性很强 
</br>
https://github.com/gclm/Hackintosh-LEGION-Y7000P-I7-9750H 
</br>
其实找了很多十代平台的EFI，包括其他品牌同款CPU i7-10875H的都不能启动，找到这里的EFI文件是唯一的一个能启动的！但定制的东西太多吧，又是9代平台的，OC的EFI在本机不能启动，试了一下clover-5144的能启动Sonoma，这才开始了从clover的修改之旅！学了一些配置知识后，才跟进OC的
</br>
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
非常感谢他们的分享！
</br>
