## 选举
zookeeper选举会有半分钟所有延迟
在重启项目时候可能会导致zk的master未释放

通过执行zk目录下zkCli.sh  进入到对应注册路径下
	ls /path
	delete /path
	完成后程序会重新进行选举
