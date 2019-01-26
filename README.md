# YONG
##wed demo for tornado

Young是一个用Python写的功能丰富的、界面小清新的类似NodeBB的社区软件。

## Features:

- 话题按主题分类，你可以查看某一主题的话题
- 支持匿名发帖，匿名评论
- 社交功能（朋友圈，发状态）
- 像QQ一样即时聊天
- 实时提醒
- 资源分享

## Installation

在Unbuntu 16.04上

    cd Young && ./scripts/install.sh

然后设置你的Mongodb环境

    1. 修改/etc/mongod.conf，添加

        replication:
            replSetName: rs0

    2. 重启Mongodb服务

        service mongod restart

    3. 启动mongo，执行initiate

        mongo
        rs.initiate()

下一步需要做的是初始化Mongodb数据库

    fab init

如果你想自己搭建Email服务器，运行setup_mail.sh脚本

    ./scripts/setup_mail.sh


