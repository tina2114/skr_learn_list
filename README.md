## 这是什么？

这是一份skr_university的学习清单，因为太菜被抓，努力学习的一份记录

# skr_learn_list

<details>
<summary>2020.10.19：DefconQuals 2018 EC3和QEMU源码解析阅读</summary>

+ [x] [DefconQuals 2018 EC3](https://github.com/tina2114/Sakura_University/tree/master/%E5%A4%96%E5%8D%A1%E8%B5%9B/DefconQuals%202018%20EC3)：mmio_write写入的位置无检测导致的UAF
  1. 无符号表，但是可以依据shift + f12搜寻class_init --> 找到realize函数 --> 找到off_xxxxx的ops结构体 --> 结构体中第一个就是mmio_read，第二个就是mmio_write
  2. write中未对写入位置进行检测，存在UAF
  3. 进行常规的伪造，将chunk创建到存储堆块的数组中，里面写入malloc的got表地址
  4. 对got里面进行改写，改成system('cat ./flag')

+ [x] [QEMU源码解析阅读](https://github.com/tina2114/Sakura_University/blob/master/QEMU%26KVM%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90%E7%AC%94%E8%AE%B0/%E7%AC%AC%E5%9B%9B%E7%AB%A0.md)：CPU虚拟化

  1. CPU虚拟化介绍

     + VMX架构，分为虚拟机监视器（VMM）和虚拟机（VM），QEMU/KVM属于VMM，挂载的镜像属于VM
     + VMCS，VCPU的描述符。用来管理VMX non-root Operation转换以及控制VCPU的行为

  2. KVM模块初始化

     初始化CPU与架构无关的数据以及设置与架构相关的虚拟化支持

  3. 虚拟机创建

     要创建虚拟机，需要用户侧的QEMU发起请求，最后将其创建的虚拟机挂载到vm_list为头节点的链表上

<details>
<summary>2020.10.20：QEMU源码解析阅读</summary>

+ [x] QEMU源码解析阅读：CPU虚拟化

  1. QEMU的CPU创建

     QEMU能模拟多种CPU，所以存在一套继承结构

     + CPU对象初始化

       CPU类型初始化(CPUState)，对象实例化(X86CPU)后，具现化(启用realize函数)

     + QEMU和KVM间的共享数据

       可能创建的最大值是三页，每页都有自己的功能，存储两者的共享数据

  2. VCPU运行

     核心代码是do-while循环，cpu运行，遇到事件需要VM Exit就退出到KVM or QEMU，根据信息进行处理，处理完毕cpu再次运行

  3. VCPU调度

     + 在同一物理CPU上运行VCPU

       VMRESUME指令

     + 需要切换到不同的物理CPU

       VMCLEAR，VMPTRLD和VMLAUNCH指令