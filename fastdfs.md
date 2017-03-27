# FastDFS

## 安装FastDFS
1. 到[官方站点](https://github.com/happyfish100)下载libfastcommon和fastdfs最新代码
2. make && make install（注意先安装libfastcommon，然后安装fastdfs）

## 修改配置文件
### storage.conf
1. store_path0
2. tracker_server

### tracker.conf
1. base_path

### cliend.conf
1. base_path
2. tracker_server 

## 启动FastDFS
1. startFdfsTracker.sh
2. startFdfsStorage.sh

## 关闭FastDFS
1. /usr/local/bin/stop.sh /usr/local/bin/fdfs_tracker
2. /usr/local/bin/stop.sh /usr/local/bin/fdfs_storage
或者以下两条命令
1. killall fdfs_trackerd
2. killall fdfs_storaged

## 重启FastDFS
1. /usr/local/bin/restart.sh /usr/local/bin/fdfs_trackered
2. /usr/local/bin/restart.sh /usr/local/bin/fdfs_storaged



