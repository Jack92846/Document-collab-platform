# Document-collab-platform
A document collaboration platform for teachers and students
# 📚 Teacher-Student Document Collaboration Management Platform

A document collaboration management and efficiency improvement tool built on Python Flask, specifically designed for teacher-student teams. It supports document version management, permission control, batch operations, file format conversion, and other functions.

## ✨ Core Features

### 📋 Document Management
- **Version control**: Complete document version history and one-click recovery
- **Permission management**: fine-grained permission control based on the RBAC model
- **Batch Operations**: Supports batch uploading, downloading, converting, and deleting of documents
- **Smart Search**: Full-text search and categorized filtering

### 🔐 User System
- **Multi-role support**: A three-tiered permission system for students, teachers, and administrators
- **Security Authentication**: JWT Token Authentication and Permission Verification
- **Personal Space**: An independent document storage space for each user

### 🛠️ File Processing
- **Format Conversion**: Supports the conversion between multiple formats, including PDF, Word, Excel, and images
- **Image optimization**: automatic compression, generation of thumbnails
- **Batch download**: Supports downloading multiple files as a ZIP package

### 📊 Collaboration Features
- **Real-time synchronization**: Real-time notification of document changes to team members
- **Operation log**: Complete operation history
- **Statistical analysis**: document access statistics and usage analysis

## 🏗️ System Architecture

### Technology stack
- **Backend framework**: Python Flask 2.3+
- **Database**: MySQL 8.0+
- **File storage**: Local file system (scalable to cloud storage)
- **Caching**: Redis (optional)
- **Deployment**: Nginx + Gunicorn


### Architecture Design
<img width="452" height="521" alt="image" src="https://github.com/user-attachments/assets/7ecb028f-6893-40ce-a75f-636d3899154f" />

## 📁 Project Structure
<img width="433" height="579" alt="image" src="https://github.com/user-attachments/assets/0e24a516-cde7-4e39-8fe1-a7b39bd7fcfe" />


## 🚀 快速开始

### 环境要求
- Python 3.8+
- MySQL 8.0+
- pip 20.0+

### 安装步骤

1. **创建项目目录**(Create project directory)
```bash
mkdir document-collab-platform
cd document-collab-platform
```
2. **创建虚拟环境**(Create a virtual environment)
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# Linux/Mac
source venv/bin/activate
```
3. **安装依赖**(Install dependencies)
```bash
pip install -r requirements.txt
```
4. **配置数据库**(Configure database)
```bash
mysql -u root -p -e "CREATE DATABASE document_management CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;"
```
5. **配置环境变量**(Configure environment variables)
```bash
cp .env.example .env
# 编辑.env文件，配置数据库连接等信息
```
6. **运行应用**(Run the application)
```bash
cd src
python app.py
```
7. **访问应用**(Access the application)
```bash
Open your browser and visit: http://localhost:5000
```

📄 License: This project adopts the MIT License. For details, please refer to the LICENSE file.

🙏 Acknowledgements: 
We would like to express our gratitude to the following open-source projects:
Flask - A concise web framework
SQLAlchemy - a powerful ORM tool
Pillow - Image Processing Library
All contributors and users
