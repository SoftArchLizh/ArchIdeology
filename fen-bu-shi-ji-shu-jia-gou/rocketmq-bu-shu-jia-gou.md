# RocketMQ 部署架构









<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>





Producer：消息的发送者；举例：发信者

&#x20;Consumer：消息接收者；举例：收信者&#x20;

Broker：暂存和传输消息；举例：邮局&#x20;

NameServer：管理Broker；举例：各个邮局的管理机构&#x20;

Topic：区分消息的种类；一个发送者可以发送消息给一个或者多个Topic；一个消息的接收者 可以订阅一个或者多个Topic消息&#x20;

Message Queue：相当于是Topic的分区；用于并行发送和接收消息





