# 🚀 3-Tier Architecture on Azure

## 📌 Overview

Designed and implemented a **production-style 3-tier architecture** on Microsoft Azure, following best practices for **scalability, security, and modular application design**.

This project demonstrates how enterprise applications are structured by separating responsibilities across independent layers.

---

## 🏗️ Architecture

### 🔹 Web Tier

* Azure Virtual Machine
* Nginx / Apache
* Public endpoint enabled
* Handles incoming client requests

### 🔹 Application Tier

* Azure Virtual Machine
* Apache Tomcat
* Private subnet
* Processes business logic

### 🔹 Database Tier

* Azure Virtual Machine
* MySQL
* Fully isolated (no public access)
* Manages persistent data

---

## 🌐 Network Design

* Virtual Network (VNet) with segmented subnets:

  * Web Subnet
  * Application Subnet
  * Database Subnet

* Network Security Groups (NSGs) enforcing controlled access

---

## 🔐 Traffic Flow & Security

| Source   | Destination | Port   | Description               |
| -------- | ----------- | ------ | ------------------------- |
| Client   | Web Tier    | 80, 22 | HTTP & SSH access         |
| Web Tier | App Tier    | 8080   | Application communication |
| App Tier | DB Tier     | 3306   | Database connectivity     |

✔ Strict **port-based access control**
✔ **Private IP communication** between tiers
✔ Database tier completely isolated from public access

---

## ✨ Key Highlights

* Secure and modular **multi-tier architecture**
* Follows **least privilege access principle**
* Designed for **scalability and maintainability**
* Aligns with **real-world cloud architecture patterns**

---

## 📂 Project Structure

* Architecture Diagram
* Deployment & Configuration Steps
* Network and Security Setup

---

## 🚀 Future Enhancements

* Integration with Load Balancer
* Auto Scaling setup
* Monitoring with Azure Monitor
* Transition to PaaS services

---

## 👨‍💻 Author

**NVSSC8**
