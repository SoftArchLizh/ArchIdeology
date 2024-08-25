# 为什么 Redis 这么快

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

1. Redis 是基于 RAM 的数据存储。RAM 访问速度至少比随机磁盘访问快 1000 倍。
2. Redis 利用 IO 多路复用和单线程执行循环来提高执行效率。
3. Redis 利用几种高效的底层数据结构。

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

