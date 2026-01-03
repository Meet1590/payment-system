# 💳 Payment System & Currency Conversion Platform (Django, SQL, REST APIs)
### End-to-End Transaction Processing & Financial Data Modeling Project

## 📌 Overview
This project implements a **secure payment processing backend** that enables registered users to send and receive payments, create payment requests, and track transaction states. The system is designed with a strong emphasis on **data integrity, auditability, and extensibility**, making it suitable as a foundation for **financial analytics and ML-driven applications**.

## Tech Stack
**Language**: Python
**Framework**: Django, Django REST Framework
**Database**: SQLite (relational schema)
**Architecture**: REST APIs, MVC pattern
**Security**: Django authentication, SSL-enabled local server  

## 🚀 Key Features
- 👤 User registration and authentication
- 💸 Peer-to-peer payment transactions
- 📩 Payment request workflow (request → approve / reject)
- 🌍 Multi-currency transaction support
- 🔄 Transaction lifecycle states:
  - `Pending`
  - `Accepted`
  - `Rejected`
- 🕒 Timestamped, audit-ready transaction records
- 🔌 RESTful APIs using Django REST Framework
- 🛠 Admin panel for transaction monitoring and management

## 🧱 System Architecture
currencyConverterApp/
│
├── payapp/ # Core payment & transaction logic
├── register/ # User registration & authentication
├── currencyConverterApp # Project configuration
├── db.sqlite3 # Relational database
├── manage.py
└── requirements.txt

**Architecture Style:**  
- MVC pattern (Django)
- REST-based backend services
- Relational data modeling

## 🛠 Tech Stack

- **Language:** Python  
- **Framework:** Django, Django REST Framework  
- **Database:** SQLite (relational schema)  
- **APIs:** REST APIs, MVC pattern
- **Security:** Django authentication, SSL-enabled local server  

## 🗂 Data Model Highlights
The system is designed around **financial transaction integrity**.

### Core Entities
- **CustomUser**
- **Transaction**
- **PaymentRequest**

### Transaction Attributes
- Sender and receiver (relationally linked users)
- Transaction amount
- Currency type
- Status (`Pending`, `Accepted`, `Rejected`)
- Creation timestamp

> This structure enables reliable **financial traceability**, regulatory-style audits, and analytics use-cases.


## 📊 Analytics & ML Readiness
While no machine learning models are implemented, the system is **intentionally designed to support data science workflows**, including:

- 📈 Transaction frequency & volume analysis
- 🧠 User behavior profiling
- 🚨 Fraud and anomaly detection
- ⏱ Time-series financial analysis
- 🌍 Currency flow and exposure analysis

All transactions are **labeled, timestamped, and relationally consistent**, making them immediately usable for supervised and unsupervised learning tasks.

## 🎯 Project Motivation
The goal of this project was to simulate the backend logic of a real payment system while applying **data-centric and analytics-driven thinking**.  
Special attention was given to how transaction data is generated, validated, and stored — a critical requirement for **fintech, risk, and analytics platforms**.

## ▶️ Getting Started
### Prerequisites
- Python 3.11.8
- Virtual environment (recommended)

### Installation
```bash
git clone <repository-url>
cd payment-system
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
