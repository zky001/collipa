collipa
=======
## 简介

The source of <http://collipa.com>

## 配置

修改 collipa/config.py 文件：

### 数据库

- _DBUSER = "username" # 数据库用户名
- _DBPASS = "password" # 数据库密码
- _DBHOST = "localhost" # 数据库地址
- _DBNAME = "collipa" # 数据库名称

### 邮箱

- _SMTPUSER = 'example@gmail.com' # 邮箱用户名
- _SMTPPASS = 'password' # 邮箱密码
- _SMTPHOST = 'smtp.gmail.com' # 邮箱地址
- _SMTPPORT = '587' # 邮箱端口

## 安装必要扩展包

### 安装 memcached

```
sudo apt-get install memcached
```

### 安装 pony

```
git clone https://github.com/ponyorm/pony
cd pony
sudo python setup.py install
```

### 安装其他

```
python setup.py --install
```

## 初始化数据库

```
python setup.py --init
```

## 运行

```
python app.py
```