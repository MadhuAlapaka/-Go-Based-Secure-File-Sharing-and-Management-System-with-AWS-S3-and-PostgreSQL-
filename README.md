# "Go-Based Secure File Sharing and Management System with AWS S3 and PostgreSQL"- File Sharing & Management System 🚀

## Overview

This project is a backend system designed for secure file sharing and management. Built using **Go (Golang)**, it integrates **PostgreSQL**, **Redis**, and **AWS S3** for efficient and scalable file handling. The system offers **user authentication**, **file upload/download capabilities**, **search functionality**, **rate limiting**, and **automatic cleanup** of expired files, all while ensuring secure file storage with encryption.

---

## 📌 Features

- ✅ **User Authentication (JWT-based)**: Secure login and registration with JWT tokens for user authentication.
  
- ✅ **File Upload & Download (AWS S3)**: Secure file uploads to and downloads from AWS S3 storage.
  
- ✅ **File Search**: Search files by **name**, **date**, and **type** for easy retrieval.
  
- ✅ **Rate Limiting**: Limit to **100 requests per minute per user** to ensure fair usage and avoid server overload.
  
- ✅ **Background Cleanup Job**: Automatically deletes expired files based on their expiration date to manage storage.
  
- ✅ **File Encryption**: All files are encrypted before upload to ensure confidentiality and integrity.
  
- ✅ **Real-time Upload Notifications (WebSockets)**: Push notifications to notify users when a file has been successfully uploaded.

---

## 🔧 Tech Stack

- **Backend**: Go (Golang)
  
- **Database**: PostgreSQL
  
- **Caching**: Redis
  
- **Storage**: AWS S3
  
- **Authentication**: JWT
  
- **Testing**: Go Unit Tests
  
- **Deployment**: Docker & GitHub

---

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository

```sh
git clone https://github.com/MadhuAlapaka/21MIS7022_Backend.git
cd 21MIS7022_Backend
2️⃣ Configure Environment
Create a .env file in the root directory and add the required credentials:

dotenv
Copy code
DB_HOST=your_database_host
DB_PORT=5432
DB_USER=your_database_user
DB_PASSWORD=your_database_password
DB_NAME=your_database_name

AWS_ACCESS_KEY_ID=your_aws_access_key_id
AWS_SECRET_ACCESS_KEY=your_aws_secret_access_key
AWS_S3_BUCKET_NAME=your_s3_bucket_name

JWT_SECRET_KEY=your_jwt_secret_key
3️⃣ Run the Project
Run the following commands to install dependencies and start the application:

sh
Copy code
go mod tidy
go run main.go
4️⃣ Run Tests
To run the unit tests:

sh
Copy code
go test ./tests/...
📌 API Endpoints
Method	Endpoint	Description
POST	/register	Register a new user
POST	/login	User login (JWT-based authentication)
POST	/upload	Upload a file to the server
GET	/files	List all files
GET	/files/{id}	Download a file by ID
DELETE	/files/{id}	Delete a file by ID

🤝 Contributing
Want to improve this project? Feel free to create a pull request!

📧 Contact
If you have any questions or would like to get in touch:

10. Author
Name: Madhu Alapaka

Email: alapakamadhusudhanbabu786@gmail.com

LinkedIn: LinkedIn Profile
