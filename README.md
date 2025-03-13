
# 🚀 DeepInsight Codemind 安装指南 / Installation Guide

---

## 🇨🇳 中文安装步骤

### 第 1 步：在服务器或本地计算机上安装 Docker  
选择适合的操作系统，并按照以下链接进行安装：  
👉 [Docker 安装指南](https://docs.docker.com/engine/install/)

### 第 2 步：打开项目文件夹并启动终端  

### 第 3 步：在 `.env` 文件中更新 Kafka 的 IP 或域名  

根据实际情况修改该值：  
- 本地网络 → 填写局域网 IP  
- 外部网络 → 填写公网 IP

```env
KAFKA_DOCKER_HOST_IP=192.168.0.191
```

### 第 4 步：启动系统  

运行以下命令启动系统：  

```bash
docker-compose up -d
```

### 第 5 步：访问系统  

打开浏览器，访问： [http://localhost:19007/](http://localhost:19007/)  
使用以下凭据登录：

- 邮箱：`admin@mail.com`  
- 密码：`uIrdowYEyUB8bTi2a1Bdd9ZpYkBJsnmL`

### 第 6 步：配置用户和仪表盘  

请参考文档：**《Setup user and dashboard - 设置用户和仪表盘.docx》**

---

## 🇬🇧 English Installation Steps

### Step 1: Install Docker on the Server or Local Machine  
Choose the appropriate platform to install Docker from the following link:  
👉 [Docker Installation Guide](https://docs.docker.com/engine/install/)

### Step 2: Open the Project Folder and Start the Terminal  

### Step 3: Update the Kafka IP or Domain in the `.env` File  

Modify the value based on the LAN IP (if using a local network) or the public IP (if using an external network):

```env
KAFKA_DOCKER_HOST_IP=192.168.0.191
```

### Step 4: Start the System  

Run the following command to launch the system:

```bash
docker-compose up -d
```

### Step 5: Access the System  

Open your browser and navigate to [http://localhost:19007/](http://localhost:19007/), then log in using the following credentials:

- **Email:** admin@mail.com  
- **Password:** uIrdowYEyUB8bTi2a1Bdd9ZpYkBJsnmL  

### Step 6: Configure Users and Dashboard  

Refer to the document **'Setup user and dashboard - 设置用户和仪表盘.docx'** for instructions on setting up users and the dashboard.
