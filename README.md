# ProtoHub Docker Compose 部署仓库

## 如何使用？

### 创建环境文件并修改

```bash
cp .env.example .env
```

```properties

# content of .env file

MYSQL_HOST=host.docker.internal # 默认宿主域名，可根据实际情况修改
MYSQL_USER_NAME=  # 数据库用户名
MYSQL_PASSWORD=   # 数据库密码
DATABASE_NAME=proto-hub  #数据库名称，建议`proto-hub`
FILE_UPLOAD_DIR=/data  # 文件上传目录
FRONTEND_HOST_NAME=localhost  #服务域名，如果本地localhost即可，支持多个域名空格分割
```

### 运行

```bash
docker compose up -d
```

### 访问

访问 http://localhost:8081

