## 这是什么？

这是一份skr_university的学习清单，因为太菜被抓，努力学习的一份记录

# skr_learn_list

<details>
<summary>2020.10.19：DefconQuals 2018 EC3和QEMU源码解析阅读</summary>

 DefconQuals 2018 EC3](https://github.com/tina2114/Sakura_University/tree/master/%E5%A4%96%E5%8D%A1%E8%B5%9B/DefconQuals%202018%20EC3)：mmio_write写入的位置无检测导致的UAF

1. 无符号表，但是可以依据shift + f12搜寻class_init --> 找到realize函数 --> 找到off_xxxxx的ops结构体 --> 结构体中第一个就是mmio_read，第二个就是mmio_write
2. write中未对写入位置进行检测，存在UAF
3. 进行常规的伪造，将chunk创建到存储堆块的数组中，里面写入malloc的got表地址
4. 对got里面进行改写，改成system('cat ./flag')

 [QEMU源码解析阅读](https://github.com/tina2114/Sakura_University/blob/master/QEMU%26KVM%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90%E7%AC%94%E8%AE%B0/%E7%AC%AC%E5%9B%9B%E7%AB%A0.md)：CPU虚拟化

