spring boot整合lettuce

lettuce基于netty，并发访问保证线程安全

但是lettuce的拓扑刷新默认关闭,在集群一台实例挂掉后，程序会报连接错误消息

解决方案：代码开启拓扑刷新

## git
https://github.com/lettuce-io/lettuce-core/wiki/Redis-Cluster#user-content-refreshing-the-cluster-topology-view


## sds