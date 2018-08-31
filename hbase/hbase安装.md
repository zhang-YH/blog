 # hbase安装
 
 ## 单机版
 
 * #### 从阿里云镜像站现在HBase安装包
 [https://mirrors.aliyun.com/apache/hbase/2.0.1/](https://mirrors.aliyun.com/apache/hbase/2.0.1/)
 
 * #### 解压缩到服务器目录/usr/local
 `tar -zxvf hbase-2.0.1-bin.tar.gz`
 
 * #### 修改conf/hbase-env.sh
 ```
 export JAVA_HOME=/usr/java/jdk.1.8.0_181/
 export HBASE_MANAGES_ZK=true
 ```
 
 * #### 修改conf/hbase-site.xml
 ```
 <configuration>
	<property>
		<name>hbase.rootdir</name>
		<value>file:/usr/local/hbase-2.0.1</value>
	</property>
</configuration>
```

* #### 启动hbase
`./bin/start-hbase.sh`

* #### 检验hbase是否正常启动
` 在bin目录执行./hbase shell,正常的话就会进入hbase命令行模式, 即hbase(main):001:0>，至此单机版hbase启动成功
 