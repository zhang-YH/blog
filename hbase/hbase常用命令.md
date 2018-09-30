# hbase常用命令

### 进入hbase命令行模式
```
首先启动hbase,使用命令./bin/start-hbase.sh
然后进入hbase命令行模式,使用命令./bin/hbase shell
```

### 表的操作

* 查看所有表
```
hbase(main):001:0>list
```

* 创建表
```
hbase(main):001:0>create '表名',{NAME=>'列族',VERSION=>'1'
```





ERROR: Table test1 is enabled. Disable it first.