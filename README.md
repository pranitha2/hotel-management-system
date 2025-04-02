Hotel Management System

Overview

The Hotel Management System is a highly scalable and secure online reservation platform, designed to facilitate hotel bookings and management. Built using Java Spring Boot for the backend and React for the frontend, this application ensures seamless user experience, robust authentication, and efficient resource management.

Features

Online Room Booking – Users can search, view, and reserve rooms in real-time.

User Authentication & Authorization – Secure login/logout system implemented with JWT authentication.

Image Management – Hotel images stored and managed using AWS S3.

Database Management – Uses AWS RDS (MySQL) for efficient data storage and retrieval.

Load Balancing – AWS Load Balancer distributes incoming traffic evenly for optimized performance.

Caching Optimization – Integrated AWS ElastiCache with Redis for improved response times.

Scalable Deployment – Hosted on AWS EC2 instance for high availability and scalability.

Tech Stack

Backend

Java Spring Boot – REST API development

MySQL (AWS RDS) – Database management

JWT Authentication – Secure user authentication

Redis (AWS ElastiCache) – Caching for improved performance

Frontend

React.js – User-friendly and responsive UI

Cloud & Deployment

AWS EC2 – Hosting the application

AWS Load Balancer – Distributing traffic

AWS S3 – Image storage

AWS RDS – Managed database

Docker & Kubernetes (Optional) – For containerization and orchestration

Setup Instructions

Prerequisites

Ensure you have the following installed on your system:

Java 11+

Spring Boot

MySQL

Node.js & npm

AWS CLI (for cloud deployment)

Backend Setup

Clone the repository:

git clone https://github.com/pranitha2/hotel-management-system.git
cd hotel-management-system/backend

Configure the database in application.properties:

spring.datasource.url=jdbc:mysql://your-aws-rds-instance:3306/hotel_db
spring.datasource.username=your-username
spring.datasource.password=your-password

Build and run the backend:

mvn clean install
mvn spring-boot:run

Frontend Setup

Navigate to the frontend directory:

cd ../frontend

Install dependencies:

npm install

Start the frontend server:

npm start

Deployment on AWS

Deploy the backend on AWS EC2.

Use AWS Load Balancer to handle incoming traffic.

Store images in AWS S3 and enable caching with AWS ElastiCache (Redis).

Set up AWS RDS (MySQL) for data management.

Future Enhancements

Implement payment gateway integration for online transactions.

Add admin dashboard for hotel managers to manage bookings and availability.

Optimize serverless architecture using AWS Lambda.
