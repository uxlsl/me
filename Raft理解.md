# Raft 理解



**Raft**是一个[共识算法](https://zh.wikipedia.org/wiki/共識演算法)

- 领袖选举（英语：Leader Election）
- 记录复写（英语：Log Replication）
- 安全性（英语：Safety）



## 领袖选举

+ 选举超时，指追随者等待成为候选人的时间
+ 候选人获得多数选票，他就成为领袖
+ 领袖发送追加信息条目



### 分裂投票

多数选票 才能结束





## 记录复写

领袖作用: 所有改变都经过领袖来完成，这个过程叫日志复制





The candidate becomes the leader if it gets votes from a majority of nodes.

This process is called *Leader Election*.

All changes to the system now go through the leader.

This process is called *Log Replication*.

Leader Election

Once we have a leader elected we need to replicate all changes to our system to all nodes.



## 参考

http://thesecretlivesofdata.com/raft/

