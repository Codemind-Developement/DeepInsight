## DeepInsight Codemind

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
