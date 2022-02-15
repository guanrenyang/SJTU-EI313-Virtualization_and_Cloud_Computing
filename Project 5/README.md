## 作业要求

Choose one of DPDK performance test and  SPDK performance test. Welcome to choose both, but no extra score.

**DPDK performance test:**

  (1)Create two virtual machines on KVM.

  (2)Compile and install DPDK library on each virtual machine.

  (3)Compile and run DPDK sample application `l2fwd` on VM2, then compile and run `pktgen-dpdk` on VM1. `pkgen-dpdk` will record the size of the packages VM1 sends and the amount of packages received from VM2, while `l2fwd` just send back the packages it received from VM1.

  (4)Evaluate DPDK’s performance of L2 forwarding.

## 报告内容

得分：25/30

本作业新建了一个VMware虚拟机，使用`libvirt`图形化界面进行配置

**相信我，这一定比用`qemu`命令行简单许多许多！**

* 建立网桥的方法（不能使用NAT，也不能使用`libvirt`自带的网桥）
* 编译安装 `DPDK`
* 运行 `l2fwd`
* 编译运行 `pktgen-dpdk`——_使用 `meson` 和 `ninja`_
* 评估`DPDK`的 _L2转发 (数据链路层转发)_ 性能  

