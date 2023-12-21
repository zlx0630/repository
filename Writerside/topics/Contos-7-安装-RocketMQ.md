# Centos 7 安装 RocketMQ

## 1. MQ下载目录

<a href="https://mirrors.tuna.tsinghua.edu.cn/apache/rocketmq/">选择适合的版本</a>

## 2. 解压

```shell
unzip rocketmq-all-5.1.2-bin-release.zip 
```

## 3. 修改内存, 自带的太大

修改为1G

```shell
vim /bin/runserver.sh
```

```shell
vim /bin/runbroker.sh
```

<tip>
    <p>
        云服务器还需要修改broker.conf
    </p>
    <p>
        新增 brokerIP1=公网IP
    </p>
</tip>

## 4. 启动

```shell
 sh mqnamesrv
```

```shell
 sh mqbroker -n 119.91.252.25:9876 -c /root/mq/rocketmq/conf/broker.conf
```