# Real-Time Fraud Detection in Financial Transactions

## Overview

This project implements a real-time fraud detection system for financial transactions using an AI-based anomaly detection technique, specifically the **Isolation Forest** model. The system continuously monitors financial transactions, detects anomalies, and flags potentially fraudulent activities in real-time.

The tool can be used by financial institutions to prevent fraudulent transactions and safeguard against financial losses.

## Features

- **Real-time Transaction Monitoring**: Continuously simulates incoming financial transactions and detects any anomalies.
- **Anomaly Detection**: The system uses the **Isolation Forest** algorithm to identify potentially fraudulent activities based on transaction patterns.
- **Interactive Dashboard**: Provides a real-time dashboard that displays:
  - Latest transactions and their fraud detection status.
  - Transaction trends over time.
  - Recently detected fraudulent transactions.
- **Historical Data**: Keeps a log of past transactions, which helps in monitoring the status of previously flagged anomalies.

## How it Works

1. **Transaction Generation**: The system generates random simulated transactions with details like amount, transaction type (credit/debit), and balance after the transaction.
2. **Data Preprocessing**: Transaction data is preprocessed, ensuring values (amount, balance) stay within valid ranges.
3. **AI Model**: The Isolation Forest model is trained on randomly generated historical data to detect outliers (fraudulent transactions). The model assigns a fraud status to each incoming transaction.
4. **Real-Time Monitoring**: Transactions are validated as they come in, and the results are displayed on the dashboard.

## Installation

To run this project locally, follow the steps below.

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/real-time-fraud-detection.git
cd real-time-fraud-detection
