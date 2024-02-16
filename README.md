# 苍穹外卖-Vichayturen改

## 1 部署流程

### 1.1 MySQL数据库
```shell
docker run -itd --name mysql57 -p 3306:3306 -p 33060:33060 -e MYSQL_ROOT_USER="root" mysql:5.7
```

### 1.2 Redis
```shell

```

### 1.3 Minio
```shell
docker run -itd --name minio -p 9000:9000 -p 9001:9001 -e MINIO_ROOT_USER="admin" -e MINIO_ROOT_PASSWORD="admin123" bitnami/minio
```

### 1.3 前端工程
下载前端工程文件，进入nginx目录，运行：
```shell
.\nginx
```

### 1.4 后端工程
maven打包运行本项目。

