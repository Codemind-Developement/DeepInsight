## DeepInsight Codemind (English)

### Step 1: Install Docker on the Server or Local Machine  

Choose the appropriate platform to install Docker from the following link:  
[Docker Installation Guide](https://docs.docker.com/engine/install/)

### Step 2: Open the Project Folder and Start the Terminal  

### Step 3: Load Docker Images  

Run the following commands to load the images into Docker:  

```sh
docker load -i ./codemind_setup/codemind_mysql.tar
docker load -i ./codemind_setup/codemind_migration.tar
docker load -i ./codemind_setup/codemind_zookeeper.tar
docker load -i ./codemind_setup/codemind_kafka.tar
docker load -i ./codemind_setup/codemind_central.tar
docker load -i ./codemind_setup/codemind_server.tar
docker load -i ./codemind_setup/codemind_admin.tar
docker load -i ./codemind_setup/codemind_watch_server.tar
```

### Step 4: Update the Kafka IP or Domain in the `.env` File  

Modify the value based on the LAN IP (if using a local network) or the public IP (if using an external network):

```env
KAFKA_DOCKER_HOST_IP=192.168.0.191
```

### Step 5: Start the System  

Run the following command to launch the system:

```sh
docker-compose up -d
```

### Step 6: Access the System  

Open your browser and navigate to [http://localhost:19007/](http://localhost:19007/), then log in using the following credentials:

- **Email:** admin@mail.com  
- **Password:** uIrdowYEyUB8bTi2a1Bdd9ZpYkBJsnmL  

### Step 7: Configure Users and Dashboard  

Refer to the document **'Setup user and dashboard - 设置用户和仪表盘.docx'** for instructions on setting up users and the dashboard.


## DeepInsight Codemind (Chinese)

### 第一步：在服务器或本地机器上安装 Docker  

选择适合的平台，在以下链接安装 Docker：  
[Docker 安装指南](https://docs.docker.com/engine/install/)

### 第二步：打开项目文件夹并启动终端  

### 第三步：加载 Docker 镜像  

运行以下命令，将镜像加载到 Docker 中：  

```sh
docker load -i ./codemind_setup/codemind_mysql.tar
docker load -i ./codemind_setup/codemind_migration.tar
docker load -i ./codemind_setup/codemind_zookeeper.tar
docker load -i ./codemind_setup/codemind_kafka.tar
docker load -i ./codemind_setup/codemind_central.tar
docker load -i ./codemind_setup/codemind_server.tar
docker load -i ./codemind_setup/codemind_admin.tar
docker load -i ./codemind_setup/codemind_watch_server.tar
```

### 第四步：在 `.env` 文件中更新 Kafka 的 IP 或域名  

根据使用的网络环境修改值：
- 若使用局域网（LAN），请使用局域网 IP。
- 若使用公共网络，请使用公网 IP。

```env
KAFKA_DOCKER_HOST_IP=192.168.0.191
```

### 第五步：启动系统  

运行以下命令启动系统：

```sh
docker-compose up -d
```

### 第六步：访问系统  

打开浏览器，访问 [http://localhost:19007/](http://localhost:19007/)，然后使用以下凭据登录：

- **电子邮件:** admin@mail.com  
- **密码:** uIrdowYEyUB8bTi2a1Bdd9ZpYkBJsnmL  

### 第七步：配置用户和仪表盘  

请参考文档 **《Setup user and dashboard - 设置用户和仪表盘.docx》**，获取有关用户和仪表盘设置的详细说明。
