
### 1. 配置信息

1. 存放nginx配置信息

> etc/nginx

2. 数据库信息(root密码, 库名, 普通用户名, 普通用户密码)放在docker-compose.yml中

### 2. 使用步骤

1. 使用git克隆docker-compose库, 并存放在当前用户目录中(即cd ~/ 所在地方)

```

git clone https://github.com/Charles-one/docker-compose.git ~/docker-compose

```

2. 复制一份执行文件到用户目录中

```

cp -r ~/docker-compose/wordpress-nginx-mariadb ~/wordpress-nginx-mariadb

```

3. 进行文件夹中, 使用docker-compose 构建镜

```

# 进行需要运行的docker-compose库中
cd ~/wordpress-nginx-mariadb

# up 表示构建, -d后台运行
# 运行后需要下载镜像, 时间比较长.
docker-compose up -d

```

4. 查看wordpress服务

访问地址:

>http://你的服务器ip

设置用户密码即可使用

5. 更多docker-compose用法[请参考这里]().


