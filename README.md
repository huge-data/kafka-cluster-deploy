
# Kafka集群部署

> Kafka版本为2.11-0.9.0.0，Zookeeper版本为3.4.6。

## 一、ZookeeperCloud

**1、安装**

./zookeeper.sh install ips

**2、启动**

./zookeeper.sh start ips

**3、查看状态**

./zookeeper.sh status ips

`注意`：有些服务器会出现“Error contacting service. It is probably not running.”错误，但是zookeeper已经正确运行。

**4、重启**

./zookeeper.sh restart ips

**5、停止**

./zookeeper.sh stop ips

**6、删除索引以及日志文件**

./zookeeper.sh deldata ips

**7、删除全部文件**

./zookeeper.sh delall ips


## 二、KafkaCloud

**1、安装**

./kafka.sh install ips

**2、启动**

`1）显示日志信息`
./kafka.sh start

`2）不显示日志信息`
./kafka.sh start &> /dev/null

**3、查看状态**

./kafka.sh status ips

**4、停止**

./kafka.sh stop ips

**5、删除索引以及日志文件**

./kafka.sh deldata ips

**6、删除全部文件**

./kafka.sh delall ips

注意事项：部署时，最好关闭防火墙。
