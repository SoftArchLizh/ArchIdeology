# CAP 定理

CAP 定理是计算机科学中最著名的理论之一，但许多开发者可能对此有不同的理解。让我们来详细了解CAP定理及其令人困惑之处。

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

CAP 定理明确指出，一个分布式系统无法同时满足以下三种保证中的两种以上。

**一致性**：一致性意味着所有客户端在连接到任何节点（系统中的服务器或计算单元）时，看到的都是相同的数据。

**可用性**：可用性意味着任何请求数据的客户端都会收到响应，即使部分节点宕机。

**分区容忍性**：分区表示两个节点之间的通信中断。分区容忍性意味着尽管存在网络分区，系统仍然继续运行。

“三者择其二”的简化公式虽然有用，**但它可能会引发误导**。

1. 选择数据库并不容易。仅仅基于 CAP 定理来证明我们的选择是远远不够的。例如，公司并不是因为 Cassandra 是 AP 系统就选择它作为聊天应用程序的数据库。还有一些良好的特性使得 Cassandra 成为存储聊天消息的理想选择。我们需要更深入地探讨。
2. “CAP 仅限制设计空间中的一小部分：在存在分区的情况下实现完美可用性和一致性，而这种情况是罕见的。” 引自论文：CAP 十二年后：规则如何改变。
3. 该定理讨论的是 100% 的可用性和一致性。更现实的讨论将是在没有网络分区的情况下，延迟和一致性之间的权衡。有关更多详细信息，请参见 PACELC 定理。

**CAP 定理是否确实有用？**

我认为它仍然是有用的，因为它使我们对一系列权衡讨论保持开放的思维，但它只是故事的一部分。我们在选择合适的数据库时需要更深入的挖掘。





