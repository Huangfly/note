# note
(1) 载入BIOS的硬件信息，并取得第一个开机装置的代号
(2)读取第一个开机装置的MBR的boot Loader (grub)的开机信息
(3)载入OS Kernel信息，解压Kernel，尝试驱动硬件
(4) Kernel执行init程序并获得run-lebel信息(如3或5)
(5) init执行/etc/rc.d/rc.sysinit
(6)启动内核外挂模块(/etc/modprobe.conf)（/etc/profile）
(7) init执行run-level的各种Scripts，启动服务
(8) init执行/etc/rc.d/rc.local
(9)执行/bin/login，等待用户Login
(10)Login后进入Shell
