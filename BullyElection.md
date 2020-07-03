# 霸道选举(Bully Election,原文“[Elections in a Distributed Computing System](http://vis.usal.es/rodrigo/documentos/papers/BullyAlgorithm.pdf)”)

## 假设（Assumption）

>* 所有节点需要合作并运行相同的算法(**All nodes cooperate and use the same election algorithm.**)

>* 每个节点的选举算法必须利用一定的软件设施。这些工具包括本地操作系统和消息处理程序。我们假设这些设施中没有“软件错误”，它们确实提供了适当的服务。(**The election algorithm at each node must
make use of certain software facilities. These facilities include a local operating system and a message handler. We assume that there are no "software bugs" in these facilities and that they indeed offer the proper services.**）

>* 如果一个节点i从节点j接收到消息M，那么该消息M在更早的时候被节点j发送到节点i。也就是说，我们假设通信子系统不会自发地生成消息。(**If a node i receives a message M from node j, then that message M was sent by node j to node i at some earlier time. That is, we assume that the communication subsystem will not spontaneously generate messages.**)

>* 

