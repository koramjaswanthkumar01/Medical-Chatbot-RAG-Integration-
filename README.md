<div align="center">

# 🏥 Hospital System RAG Chatbot

![Python Version](https://img.shields.io/badge/python-3.11-blue.svg)
![FastAPI](https://img.shields.io/badge/FastAPI-0.115.4-009688.svg)
![Neo4j](https://img.shields.io/badge/Neo4j-5.26.0-008CC1.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.39.0-FF4B4B.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

_An intelligent chatbot integrating LangChain, Neo4j, and Google Gemini to interact with hospital systems_

English | [Tiếng Việt](README.md)

</div>

## 📑 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [System Architecture](#-system-architecture)
- [Tech Stack](#-tech-stack)
- [Installation and Setup](#-installation-and-setup)
- [Project Structure](#-project-structure)
- [API Documentation](#-api-documentation)
- [Environment and Configuration](#-environment-and-configuration)
- [Docker Deployment](#-docker-deployment)
- [Testing](#-testing)
- [Contributing](#-contributing)
- [License](#-license)

## 🌟 Overview

The Hospital System RAG Chatbot is an intelligent chatbot system built to support information querying and analysis within a hospital network. The project utilizes a RAG (Retrieval-Augmented Generation) architecture combined with LangChain and Google Gemini to deliver a natural and highly accurate conversational experience.

### Key Advantages:

- 🤖 Natural interactions tailored to user language
- 📊 Real-time data analysis
- 🔄 Multi-source data integration
- 🛡️ Robust security and access control
- 📈 High scalability

## 💫 Features

### 1. Hospital Information Management

- Look up detailed hospital information
- Monitor capacity and operational status
- Analyze statistical data

### 2. Doctor and Staff Management

- Look up profiles and schedules
- Performance evaluation and feedback tracking
- Analyze expertise and experience

### 3. Patient Management

- Query medical and treatment histories
- Track costs and insurance details
- Analyze disease and medical condition patterns

### 4. Analysis and Reporting

- Wait-time statistics
- Cost and revenue analysis
- Quality assessment reports

## 🏗 System Architecture

```mermaid
graph TD
    A[Frontend - Streamlit] --> B[API Layer - FastAPI]
    B --> C[LangChain Agents]
    C --> D[Google Gemini]
    C --> E[Neo4j Database]
    B --> F[ETL Pipeline]
    F --> E
