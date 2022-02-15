## 作业要求

Hugepage in virtualization:

  (1)Prepare 2MB or 1GB hugepages on your host server. Present your hugepage configure (e.g. `/proc/meminfo`).

  (2)Create a QEMU KVM virtual machine using hugepages on the host.

  (3)Create another QEMU KVM VM without hugepages.

  (4)In both VMs allocate and use hugepages or not.

  (5)Run memory instensive benchmark(e.g. sysbench memory test, in-memory database) on two VMs and record the performance.

  (6)Compare the result and try to give some explanation.

  // Note: If the OS supports transparent huge page, disable it when you do the tests.

## 报告内容

得分：20/20

* Hugepage 的原理
* 在虚拟机上使用 Hugepage 的方法（2M和1G），和一些坑
* Sysbench 原理和使用方法
* 性能测试和原因分析