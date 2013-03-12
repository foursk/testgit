# MongoDB-Notice

##MongoDB中mongod服务的启动

1.创建数据存储目录和日志文件

    mkdir /usr/local/mongo/data 
    touch /usr/local/mongo/mongodb.log
2.启动mongod服务 **注意是否有执行和写入的权限**

    /usr/local/mongo/bin/mongod --dbpath=/usr/local/mongo/data --logpath=/usr/local/mongo/mongodb.log --logappend&

创建 `MongoDB.conf` 并将以下内配置写入文件中

    #configuration Options for MongoDB

    dbpath    = /data/db/
    logpath   = /data/log/m.log
    logappend = true


    
