# 在线教育平台

这是一个综合的在线教育平台，包含后端 API 服务器、管理员前端界面和用户前端界面。

## 项目结构

- `backend/`: 后端 API 服务器
- `frontend-admin/`: 管理员前端界面
- `frontend-user/`: 用户前端界面

## 前置要求

在运行此项目之前，请确保你的系统中已安装以下软件：

- Node.js (推荐版本 14.x 或更高)
- npm (通常随 Node.js 一起安装)
- MongoDB (确保 MongoDB 服务正在运行)

## 安装

1. 克隆仓库：

   ```bash
   git clone https://github.com/your-username/online-education-platform.git
   cd online-education-platform
   ```

2. 安装所有依赖：

   ```bash
   npm run install:all
   ```

   这个命令会安装主项目和所有子项目的依赖。

## 配置

1. 后端配置：
   - 进入 `backend/` 目录
   - 复制 `.env.example` 文件并重命名为 `.env`
   - 根据你的环境修改 `.env` 文件中的配置
在 `.env` 文件中设置以下环境变量：

     ```
     MONGO_URI=mongodb://<your_mongodb_host>:<port>/online_education_platform
     JWT_SECRET=<your_jwt_secret>
     MINIO_ENDPOINT=<your_minio_host>
     MINIO_PORT=<your_minio_port>
     MINIO_ACCESS_KEY=<your_minio_access_key>
     MINIO_SECRET_KEY=<your_minio_secret_key>

## 运行项目

1. 启动后端服务器：

   ```bash
   cd backend
   npm install
   npm run dev
   ```

   后端服务器将在 http://localhost:5000 运行（除非在 .env 文件中另有指定）。

2. 启动管理员前端：

   ```bash
   cd frontend-admin
   npm install
   npm strat
   ```

   管理员界面将在 http://localhost:3000 运行。

3. 启动用户前端：

   ```bash
   cd frontend-user
   npm install
   npm strat
   ```

   用户界面将在 http://localhost:3001 运行。

注意：请确保在不同的终端窗口中运行这些命令，因为每个命令都会持续运行并输出日志。

## 使用说明

- 访问 http://localhost:3000 进入管理员界面
- 访问 http://localhost:3001 进入用户界面
- API 文档可在 http://localhost:5000/api-docs 查看（如果已配置 Swagger）



## 联系方式

