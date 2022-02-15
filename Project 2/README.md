## 作业要求

Virtualized and bare metal network performance test. 

1. Download QEMU 5.2.0 from [https://www.qemu.org/download ](https://www.qemu.org/download/) and compile.
2. Create 2 VMs with TAP mode network(e1000 and virtio-net) by QEMU .
3. Connect to your VM through VNC viewer or SSH.
4. Compare the network （e1000 and virtio-net)）performance of your host machine and VMs.

## 报告内容

得分 18/20

* 从源码编译 `qemu` 的全过程
* `qemu` 使用方法
* `ssh` 连接虚拟机
* `vnc` 连接虚拟机
* 使用 `iperf` 比较 `e1000` 和 `virto-net` 的**网络性能**—— _`e1000`全虚拟化，`virto-net` 半虚拟化，结果应为 virto-net 优于 e1000_。

