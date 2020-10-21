## 这是什么？

这是一份skr_university的学习清单，因为太菜被抓，努力学习的一份记录

# skr_learn_list

前面因为年代久远，就以周为单位，后面再以日为单位

<details>
<summary>第一周（2020.5.18-2020.5.23）：Prime c++和stl源码剖析（视频+代码）</summary>

+ [x] Prime c++：第一章到第六章

  前面和prime c没什么太大的区别，就暂且不进行记录

+ [x] stl源码剖析

  STL是C++标准库的一部分，占据了大部分的比例。STL借助模板把常用的数据结构及其算法都实现了一遍，且做到了数据结构和算法的分离。

  + [视频总结](https://github.com/tina2114/Sakura_University/blob/master/%E7%AC%AC%E4%B8%80%E8%87%B3%E4%BA%8C%E5%91%A8/README.md)

    六大组件：

    1. 容器：

       序列容器 + 关联式容器

    2. 算法：

       sort，search，copy，erase，for_each，unique

    3. 迭代器：

       广义指针，使得算法能独立于容器

    4. 仿函数：

       泛化算法

    5. 配置器

       为容器提供空间配置和释放，对象构造和析构的服务

    6. 配接器

       将一种容器修饰为功能不同的另一种容器。例如deque，在此基础上禁用一些deque的功能实现队列和栈，这就是一种配接器。

  + [源码抄写](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B8%80%E8%87%B3%E4%BA%8C%E5%91%A8)

    </details>

<details>
<summary>第二周（2020.5.23-2020.5.29）：STL源码抄写和相应漏洞查找和小作业</summary>

+ [x] [STL源码抄写](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B8%80%E8%87%B3%E4%BA%8C%E5%91%A8)

+ [x] [相应漏洞查找](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B8%80%E8%87%B3%E4%BA%8C%E5%91%A8/%E6%80%9D%E8%80%83%E9%A2%98%E4%B8%80)

  erase的处理不当，造成的浅拷贝

+ [x] [小作业](https://github.com/tina2114/Sakura_University/blob/master/%E7%AC%AC%E4%B8%80%E8%87%B3%E4%BA%8C%E5%91%A8/%E6%B5%8B%E8%AF%95%E9%A2%98/zhz_2.md)

  </details>

<details>
<summary>第三周（2020.5.29-2020.6.05）：compiler(视频加代码）</summary>

+ [x] [Lexer-词法分析](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B8%89%E8%87%B3%E5%85%AB%E5%91%A8/PA2)

  主要编写符合cool语法的正则表达式的匹配规则，通过正则匹配对应的字符串，返回token

+ [x] [Parser-语法分析](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B8%89%E8%87%B3%E5%85%AB%E5%91%A8/PA3)

  构建一个AST抽象语法树，但是其只是token的组合，还需要进行处理

<details>
<summary>第四周（2020.6.05-2020.6.14）：compiler(视频加代码）</summary>

+ [x] [Semant-语义分析](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B8%89%E8%87%B3%E5%85%AB%E5%91%A8/PA4)

  对Parser构成的AST抽象语法树进行二次处理，设定Environment(建立各种符号表)来约束各个类，方法的作用域

+ [ ] Code generator-代码生成

  1.计算继承图

  2.以深度优先的顺序将标签分配给所有类

  3.确定每个类的属性，临时对象和调度表的布局

  4.为全局数据生成代码：常量，调度表，...

  5.为每个功能生成代码

  </details>

<details>
<summary>第五周（2020.6.14-2020.6.21）：compiler(视频加代码）和flex代码骨架分析</summary>

+ [ ] Code generator-代码生成

  未完成，学不懂了......

+ [x] [flex代码骨架分析](https://github.com/tina2114/Sakura_University/blob/master/%E7%AC%AC%E4%B8%89%E8%87%B3%E5%85%AB%E5%91%A8/lexer%E4%BB%A3%E7%A0%81%E9%AA%A8%E6%9E%B6%E6%95%B4%E7%90%86.md)

  </details>

<details>
<summary>第六周（2020.6.21-2020.6.28）：复习周 + SICP视频</summary>

+ [x] SICP视频

  一直看到了P4（复合函数）

  </details>

<details>
<summary>第七周（2020.6.28-2020.7.05）：复习周 + SICP视频</summary>

+ [x] SICP视频

  看到了P6（符号化求导程序）

  </details>

<details>
<summary>第八周（2020.7.05-2020.7.12）：实训</summary>

​	写疫情实时监控系统去了......

​	</details>

<details>
<summary>第九周（2020.7.12-2020.7.19）：csapp及其lab</summary>

+ [x] csapp：第一章到第三章

+ [x] csapp-lab：lab1到lab3

  [lab1](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B9%9D%E8%87%B3%E5%8D%81%E5%91%A8/csapp_lab/datalab)：Data lab

  使用<<，>>，^，&此类基本操作数实现取反，三位运算符，比较整数大小，浮点数转换等操作

  [lab2](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B9%9D%E8%87%B3%E5%8D%81%E5%91%A8/csapp_lab/bomb)：Bomb lab

  一些简单的汇编，还算简单，唯独parse_6需要看出链表结构。还在parse_4中存在一处隐藏关卡

  lab3：Attack lab

  入门pwn

  </details>

<details>
<summary>第十周（2020.7.19-2020.7.26）：csapp及其lab</summary>

+ [x] csapp-lab：lab4到lab7

  [lab4](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B9%9D%E8%87%B3%E5%8D%81%E5%91%A8/csapp_lab/archlab)：Arch lab

  与X86-64指令集相似的Y86-64指令集的学习，以及立即数的加入，优化。

  [lab5](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B9%9D%E8%87%B3%E5%8D%81%E5%91%A8/csapp_lab/cachelab)：Cache lab

  自行模拟一个cache，来达到高速缓存的作用。

  [lab6](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B9%9D%E8%87%B3%E5%8D%81%E5%91%A8/csapp_lab/shlab-handout)：Shell lab

  实现一个简易的linux里的shell

  [lab7](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E4%B9%9D%E8%87%B3%E5%8D%81%E5%91%A8/csapp_lab/malloclab)：Malloc lab

  实现一个简易的glibc的堆块回收

  </details>

<details>
<summary>第十一周（2020.7.26-2020.8.02）：csapp</summary>

+ [x] csapp：看到最后一章并发编程

+ [ ] csapp-lab：proxy lab

  未完成

  </details>

<details>
<summary>第十二周（2020.8.02-2020.8.09）：ucore</summary>

+ [x] ucore-lab：lab1到lab2

  [lab1](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E5%8D%81%E4%B8%80%E8%87%B3%E5%8D%81%E5%85%AD%E5%91%A8/LAB%201)：

  启动操作系统的bootloader，操作系统如何加载到内存

  [lab2](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E5%8D%81%E4%B8%80%E8%87%B3%E5%8D%81%E5%85%AD%E5%91%A8/LAB%202)：

  first-fit连续物理内存分配，寻找虚拟地址对应的页表项

  </details>

<details>
<summary>第十三周（2020.8.09-2020.8.16）：ucore</summary>

+ [x] ucore-lab：lab3到lab5

  [lab3](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E5%8D%81%E4%B8%80%E8%87%B3%E5%8D%81%E5%85%AD%E5%91%A8/LAB%203)：虚拟内存管理

  页表机制，换出机制，缺页故障处理

  [lab4](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E5%8D%81%E4%B8%80%E8%87%B3%E5%8D%81%E5%85%AD%E5%91%A8/LAB%204)：内核线程管理

  建立内核线程的关键信息

  [lab5](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E5%8D%81%E4%B8%80%E8%87%B3%E5%8D%81%E5%85%AD%E5%91%A8/LAB%205)：用户进程管理

  （创建，执行，切换，结束）

  </details>

<details>
<summary>第十四周（2020.8.16-2020.8.23）：ucore</summary>

+ [x] ucore-lab：lab6到lab7

  [lab6](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E5%8D%81%E4%B8%80%E8%87%B3%E5%8D%81%E5%85%AD%E5%91%A8/LAB%206)：进程调度

  进程一共三个状态，等待，就绪，运行，RR调度算法，Stride Scheduling调度算法

  [lab7](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E5%8D%81%E4%B8%80%E8%87%B3%E5%8D%81%E5%85%AD%E5%91%A8/LAB%207)：同步互斥

  内核级信号量的实现，哲学家就餐问题

  </details>

<details>
<summary>第十五周（2020.8.23-2020.8.30）：ucore</summary>

+ [x] ucore-lab：lab8

  [lab8](https://github.com/tina2114/Sakura_University/tree/master/%E7%AC%AC%E5%8D%81%E4%B8%80%E8%87%B3%E5%8D%81%E5%85%AD%E5%91%A8/LAB%208)：文件系统

  VFS结构，文件控制块，读文件操作的实现

  </details>

<details>
<summary>第十六周（2020.8.30-2020.9.06）：ucore</summary>

+ [x] ucore-lab拓展：lab1拓展到lab4拓展

  lab1拓展：

  1. 从用户态切换到内核态的函数

     利用int指令产生软中断，再恢复esp

  2. 内核态到用户态的互相切换

     内核态到用户态需要先获取真正的ebp和esp，再抬栈伪造esp和ss

     用户态到内核态需要先把内核态上除了ss和esp的内容全复制到原先用户态的栈上，这是为了中断返回后能够正常执行原先被打断的程序。将伪造的栈上的段寄存器进行修改，使其指向DPL为0的相应段描述符

  lab2拓展：伙伴系统分配算法

  ​	设计一个二叉树的树状结构，根节点的内存空间最大，每一层的内存空间都是上一层的一半，用户要求size大小的内存块时，会先判断是否是2的倍数，不是就向上取整，在二叉树里匹配，分配。

  在释放内存块时，会依次进行判断临近节点和父节点是否空闲，是就依次合并。

  lab3拓展：实现识别dirty bit的 extended clock页替换算法

  ​	与LRU算法类似，不过......如果真要实现的话，应该得对这个ucore进行大魔改，所以就进行了简易的实现

  lab4拓展：无拓展

  </details>

<details>
<summary>第十七周（2020.9.06-2020.9.13）：ucore和unix环境 高级编程</summary>

+ [x] ucore-lab拓展：lab5拓展到lab6拓展

  lab5拓展：实现COW机制

  ​	写时复制，只有在进行写操作的时候才分配新的物理页

  lab6拓展：CFS调度算法

  ​	主要是简化了virutime中的运行周期 * 1024 / 进程权重，转而变成 1024 / 进程权重，因为ucore本身设计是基于时间片的调度，运行周期并未在ucore中定义

+ [x] unix环境高级编程：看到第五章

  </details>

<details>
<summary>第十八周（2020.9.13-2020.9.20）：虚拟化题目复现和unix环境 高级编程</summary>

+ [x] [CONFidence ctf 2020 kvm](https://github.com/tina2114/Sakura_University/tree/master/%E5%A4%96%E5%8D%A1%E8%B5%9B/CONFidence%20ctf%202020)：

  1. 这题算不上真正的虚拟化，在程序里分配了一块区域来模拟
  2. 漏洞点主要出现在分配出来的栈起始地址和创建虚拟化时的起始地址不一致， 0x7fffffff5cc0为栈起始地址，size大小为0x8000，0x7fffffff6000为虚拟化空间起始地址，size大小也为0x8000
  3. 造成的问题是可以在虚拟化空间里获取物理机的数据，拿到ret地址
  4. 伪造页表项，进入到储存ret地址所在的地方，将ret地址改为one_gadget地址

+ [ ] PlaidCTF 2020 sandybox：

  复现到一半，还未完成

+ [x] unix环境 高级编程：看到第六章

  </details>

<details>
<summary>第十九周（2020.9.20-2020.9.27）：虚拟化题目复现和QEMU源码解析阅读</summary>

+ [x] [PlaidCTF 2020 sandybox](https://github.com/tina2114/Sakura_University/tree/master/%E5%A4%96%E5%8D%A1%E8%B5%9B/PlaidCTF%202020/sandybox)：

  1. 借用了ptrace函数来模拟实现沙盒
  2. 漏洞点在于设计模式的小问题，因为它预设的信号都是两次，子进程进行系统调用一次，系统调用结束一次。但是如果有只发生一次信号的调用存在呢？
  3. 这里就借用了int 3，系统调用信号只发送一次来进行绕过沙盒检测，来执行我们的shellcode

+ [x] [QEMU源码解析阅读](https://github.com/tina2114/Sakura_University/blob/master/QEMU%26KVM%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90%E7%AC%94%E8%AE%B0/%E7%AC%AC%E4%B8%80%E7%AB%A0.md)：

  QEMU/KVM概述

  </details>

<details>
<summary>第二十周（2020.9.27-2020.10.04）：调试器和QEMU源码解析阅读</summary>

+ [x] [调试器](https://github.com/tina2114/Sakura_University/tree/master/homework/%E8%B0%83%E8%AF%95%E5%99%A8)：

  实现了看寄存器，运行，断点功能

+ [x] [QEMU源码解析阅读](https://github.com/tina2114/Sakura_University/blob/master/QEMU%26KVM%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90%E7%AC%94%E8%AE%B0/%E7%AC%AC%E4%BA%8C%E7%AB%A0.md)：第二章

  1. 先去用c实现了一下OOP的三种最基本的特性：封装，继承，多态

  2. glib事件循环机制

     glib实现了完整的事件循环分发机制，一次循环包括prepare，query，check，dispatch过程

  3. QEMU事件循环机制

     glib_pollfds_fill，qemu_poll_ns，glib_pollfds_fill

     </details>

<details>
<summary>第二十一周（2020.10.04-2020.10.11）：虚拟化题目复现和QEMU源码解析阅读</summary>

+ [x] [blizzardctf2017 strng](https://github.com/tina2114/Sakura_University/tree/master/%E5%A4%96%E5%8D%A1%E8%B5%9B/blizzardctf2017)：pmio_write写入位置未检测导致的越界

  1. pmio_read进行越界读，将结构体里面buf后面跟着的srand函数地址读出来
  2. 计算libc基址和system地址
  3. 将指针覆盖成system，再写入"cat /root/flag"作为参数，调用指针

+ [x] [HITB GSEC 2017 babyqemu](https://github.com/tina2114/Sakura_University/tree/master/%E5%A4%96%E5%8D%A1%E8%B5%9B/HITB%20GSEC%202017)：同样的未检测导致的越界

  和上面的题目差不多，也是结构体里的buf后面跟着一个指针，读取指针，拿到程序基址，再拿到system_plt地址，后面就是把指针覆盖成system_plt地址，写入参数，调用

+ [ ] [QEMU源码解析阅读](https://github.com/tina2114/Sakura_University/blob/master/QEMU%26KVM%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90%E7%AC%94%E8%AE%B0/%E7%AC%AC%E4%B8%89%E7%AB%A0.md)：第三章

  未完成

  </details>

<details>
<summary>第二十二周（2020.10.11-2020.10.18）：cve-2015-5165复现和QEMU源码解析阅读</summary>

+ [x] [cve-2015-5165](https://github.com/tina2114/Sakura_University/tree/master/%E6%BC%8F%E6%B4%9E%EF%BC%8Cparttern%E5%88%86%E6%9E%90/qemu-pwn-cve-2015-5165)：典型的整数下溢

+ [x] [QEMU源码解析阅读](https://github.com/tina2114/Sakura_University/blob/master/QEMU%26KVM%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90%E7%AC%94%E8%AE%B0/%E7%AC%AC%E4%B8%89%E7%AB%A0.md)：第三章

  1. fw_cfg设备

     fw_cfg完成把QEMU数据传递给虚拟机的工作

  2. SeaBIOS

     SeaBIOS是QEMU/KVM虚拟化方案的默认BIOS

+ [ ] DefconQuals 2018 EC3：

  未完成

  </details>

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
     
     </details>

<details>
<summary>2020.10.20：QEMU源码解析阅读</summary>
+ [x] [QEMU源码解析阅读](https://github.com/tina2114/Sakura_University/blob/master/QEMU%26KVM%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90%E7%AC%94%E8%AE%B0/%E7%AC%AC%E5%9B%9B%E7%AB%A0.md)：CPU虚拟化

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
       
       </details>

