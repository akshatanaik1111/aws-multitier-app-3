# aws-multitier-app-3
# Multi-tier Web Application

# Multi-tier Web App Deployment

## 📌 Project Overview

This project demonstrates how to deploy a multi-tier web application on AWS using Amazon EC2, Amazon RDS, and Load Balancer.

The application architecture is divided into three separate layers:

- Frontend Layer
- Backend Layer
- Database Layer

This separation improves scalability, security, performance, and maintainability of the application.

The project helps in understanding real-world cloud architecture used in modern enterprise applications.

---

# 🎯 Objective

- Build scalable application architecture
- Separate frontend, backend, and database
- Improve application security
- Enable high availability
- Understand multi-tier deployment concepts

---

# 🧰 AWS Services Used

## 1. Amazon EC2
Used to host frontend and backend application servers.

## 2. Amazon RDS
Used to manage relational database services.

## 3. Load Balancer
Used to distribute incoming traffic across application servers.

## 4. Security Groups
Used to secure communication between tiers.

## 5. AWS VPC
Provides isolated networking environment.

---

# 🏗️ Multi-tier Architecture

The application is divided into three layers:

## 1. Frontend Layer

- Handles user interface
- Receives client requests
- Hosted on EC2 instance

## 2. Backend Layer

- Processes application logic
- Communicates with database
- Hosted on EC2 instance

## 3. Database Layer

- Stores application data
- Managed using Amazon RDS

---

# ⚙️ Step-by-Step Implementation

## Step 1: Create VPC

- Open AWS Console
- Go to VPC Dashboard
- Create custom VPC
- Configure subnets
- Configure Internet Gateway

---

## Step 2: Launch Frontend EC2 Instance

- Go to EC2 Dashboard
- Launch EC2 instance
- Install web server
- Configure frontend application

---

## Step 3: Launch Backend EC2 Instance

- Create another EC2 instance
- Configure backend application
- Enable communication with database

---

## Step 4: Create Amazon RDS Database

- Go to RDS Dashboard
- Create database
- Select MySQL/PostgreSQL
- Configure username and password
- Enable database connectivity

---

## Step 5: Configure Security Groups

Allow:

### Frontend Security Group
- HTTP (Port 80)
- HTTPS (Port 443)

### Backend Security Group
- Application Port Access

### Database Security Group
- MySQL Port 3306

---

## Step 6: Create Load Balancer

- Go to EC2 Dashboard
- Select Load Balancers
- Create Application Load Balancer
- Add listeners
- Attach Target Group

---

## Step 7: Configure Target Group

- Register frontend/backend instances
- Enable health checks

---

## Step 8: Connect Application with Database

Configure backend application to connect with RDS database.

---

## Step 9: Test Application

- Copy Load Balancer DNS
- Open in browser
- Verify frontend, backend, and database connectivity

---

# 📸 Project Screenshots

## 🔹 Frontend EC2 Instance

<img width="1922" height="1083" alt="Frontend server (browser)" src="https://github.com/user-attachments/assets/b067d1f0-ed1b-411a-837a-ab1536df4cc0" />

<img width="1922" height="1023" alt="frontend server calling to Backend" src="https://github.com/user-attachments/assets/b88b7f44-756a-40bb-a227-d0d2ec121dc6" />

---

## 🔹 Backend EC2 Instance
<img width="1923" height="1023" alt="Backend server" src="https://github.com/user-attachments/assets/ad3cc728-653f-4814-8148-54b874917159" />

<img width="1923" height="1023" alt="BE server (open in browser)" src="https://github.com/user-attachments/assets/6204f3ec-4df1-4b47-9c3e-48c95aed2757" />

---

## 🔹 Amazon RDS

<img width="1923" height="1012" alt="Database name of RDS mydb" src="https://github.com/user-attachments/assets/c7e54f97-d5f4-4bed-b887-ef0adac87fcf" />

---

## 🔹 Load Balancer


<img width="1921" height="1017" alt="Load balancer" src="https://github.com/user-attachments/assets/9e20235d-1685-4f20-9b2b-3971af558422" />

---

## 🔹 Security Groups

![Security Groups](Security%20Groups.png)

---

## 🔹 Target Group

<img width="1923" height="1023" alt="Target Group" src="https://github.com/user-attachments/assets/2308ce08-f0cd-4a13-9598-42c2ba18fdfc" />

---

## 🔹 Application Output

<img width="1922" height="1023" alt="frontend server calling to Backend" src="https://github.com/user-attachments/assets/b88b7f44-756a-40bb-a227-d0d2ec121dc6" />

<img width="1923" height="1023" alt="Backend server" src="https://github.com/user-attachments/assets/ad3cc728-653f-4814-8148-54b874917159" />

<img width="1923" height="1022" alt="DB is created in BE server" src="https://github.com/user-attachments/assets/dbc13b1e-d077-4952-b4bf-c6e91750eda0" />

<img width="1923" height="1018" alt="Table is created in BE server" src="https://github.com/user-attachments/assets/cd06fa10-4379-4b94-8d2e-e99461b80fc6" />

---

# ✅ Features

- Multi-tier architecture
- Improved scalability
- Better security
- Database integration
- Traffic distribution
- High availability
- Fault tolerance

---

# 📚 Learning Outcomes

Through this project, I learned:

- Multi-tier application architecture
- EC2 instance configuration
- Amazon RDS setup
- Load Balancer configuration
- Security Group management
- Database connectivity
- Scalable cloud deployment concepts

---

# 🚀 Future Improvements

- Add Auto Scaling
- Configure HTTPS
- Add CloudWatch Monitoring
- Implement CI/CD Pipeline
- Add Route 53 Domain Mapping

---

# 🏁 Conclusion

This project successfully demonstrates deployment of a multi-tier web application on AWS using EC2, RDS, and Load Balancer. The architecture improves scalability, security, and maintainability by separating application layers.

---

# 👩‍💻 Author

Akshata Naik

---
