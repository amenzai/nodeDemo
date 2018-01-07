一个 `node + express + mongodb` demo

## 使用方法

**下载项目：**

```bash
git clone https://github.com/amenzai/nodeDemo.git
cd nodeDemo
npm install
npm start
```

**使用mongodb：**

首先下载MongoDB：http://www.mongodb.org/downloads。

安装完以后，找到安装目录，比如`D:\mongodb\bin`(可以将其配置到环境变量)

然后
```bash
# 设置数据库目录
mongod --dbpath 'C:\data\db'

# 新开个命令行
mongo

# 使用数据库
use test-mongo

# 插入一条数据
db.usercollection.insert({ "username" : "chao", "email" : "chao@testdomain.com" })

# 查看插入的数据
db.usercollection.find().pretty()
```

## 功能简要介绍

路由（地址栏输入即可）：

- /newuser：添加用户
- /userlist：查看用户列表

用到的接口：

- /adduser：添加用户接口