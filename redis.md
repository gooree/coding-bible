#Redis

# 安装
1. 到redis官方站点下载最新稳定的发布版本安装包
2. 解压安装包
3. make && make install

# 配置
1. 访问密码

打开/etc/redis/redis.conf，找到以requirepass指令开头的行，删除注释符号，并修改requirepass指令后的密码。（注：集群环境下slave节点也要配置相应的密码）

2. 绑定IP

打开/etc/redis/redis.conf，在bind指令后添加绑定的ip即可。

# 启动
redis-server /etc/redis/redis.conf

# 连接
redis-cli

# 关闭
redis-cli shutdown
