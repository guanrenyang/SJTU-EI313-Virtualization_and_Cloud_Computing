# `libvirt` 图形化界面配置

1. 新版`libvirt`不支持旧版 `qemu`，因此最好 **开一个新的虚拟机** 重新安装或者 **删除`qemu`**。

   _笔者新开了一个虚拟机，因此不知道起冲突的到底是什么。_

2. 确保CPU支持虚拟化  

   ```shell
   grep -Eoc '(vmx|svm)' /proc/cpuinfo
   ```

   有输出说明支持虚拟化

3. 安装`qemu-kvm`

   ```shell
   sudo apt install qemu-kvm
   ```

   不需要安装完整`qemu`，只需要安装`qemu-kvm`即可。

4. 安装必要文件 

   ```shell
   sudo apt install libvirt-daemon-system
   sudo apt install libvirt-clients
   sudo apt install bridge-utils
   sudo apt install virtinst
   sudo apt install virt-manager
   ```

   `libvirt-daemon-system` 将 `libvirt `守护程序作为系统服务运行的配置文件。

   `libvirt-clients` 用来管理虚拟化平台的软件。 

   `bridge-utils` 用来配置网络桥接。 

   `virtinst `用来创建虚拟机的命令行工具。 

   `virt-manager` 提供一个图形界面管理虚拟机  

