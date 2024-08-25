# 支撑您的数据库的8种数据结构

答案会根据您的使用情况而有所不同。数据可以在内存或磁盘上进行索引。类似地，数据格式各异，例如数字、字符串、地理坐标等。系统可能是写重型或读重型。所有这些因素都会影响您选择的数据库索引格式。

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

以下是一些最常用的用于数据索引的数据结构：

* 跳表：一种常见的内存索引类型。在Redis中使用

&#x20;       &#x20;

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

* 哈希索引：一种非常常见的“映射”数据结构（或“集合”）的实现
* SSTable：不可变的磁盘“映射”实现
* LSM树：跳表 + SSTable。高写入吞吐量
* B树：基于磁盘的解决方案。稳定的读/写性能
* 倒排索引：用于文档索引。在Lucene中使用
* 后缀树：用于字符串模式搜索
* R树：多维搜索，例如寻找最近邻









