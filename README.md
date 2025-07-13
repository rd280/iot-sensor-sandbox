# IoT Sensor Sandbox

A cloud-native sandbox project simulating IoT sensor data ingestion, storage, and visualization using AWS services and a React dashboard.

---

## Project Overview

This project simulates temperature and humidity sensor data that is sent to AWS IoT Core. The data flows through AWS Lambda functions and is stored in DynamoDB. A React-based dashboard displays the sensor data in real-time charts.

---

## Tech Stack

- **AWS IoT Core** — MQTT device connectivity and message routing  
- **AWS Lambda** — Serverless functions for data processing and retrieval  
- **Amazon DynamoDB** — NoSQL database for sensor data storage  
- **React + Next.js (via Vercel v0)** — Frontend dashboard for data visualization  
- **Python** — Sensor simulator and Lambda function code  
- **GitHub & Vercel** — Version control and frontend deployment  

---

## Features

- Simulated sensor data publishing to AWS IoT Core  
- Serverless ingestion and storage of sensor readings  
- REST API endpoints to fetch latest sensor data  
- Responsive React dashboard with charts and data tables  
- Easily extendable for real IoT device integration or advanced AWS features  

---

## Project Structure

iot-sensor-sandbox/
├── frontend/ # React/Next.js dashboard (generated with v0)
├── backend/ # AWS Lambda functions (store and get sensor data)
│ ├── lambda_store_data/
│ └── lambda_get_data/
├── simulator/ # Python script simulating sensor data publishing
├── infra/ # (Optional) Infrastructure as Code scripts
├── README.md
└── .gitignore


---

## Getting Started

### Prerequisites

- Node.js & npm  
- Python 3.x  
- AWS Account with IoT Core, Lambda, and DynamoDB access  
- AWS CLI (optional, for deployment)  
- Vercel account (for frontend deployment)  

### Installation

1. Clone the repo  
```bash
git clone https://github.com/your-username/iot-sensor-sandbox.git
cd iot-sensor-sandbox
