# Thndr Data Engineering Use Case

This repository contains a complete data engineering analysis of **Thndr**, a digital investment platform operating in the Egyptian market. The project breaks down how Thndr might use data across different layers of a modern data engineering pipeline.

## Overview
This analysis covers:
- Data Sources  
- Storage Layer  
- Processing Layer  
- Serving Layer  
- Abstracted Data Pipeline Diagram  

The goal is to understand how a real-world fintech platform structures its data systems to support analytics, reporting, and real-time decision-making.

## Data Sources
Thndr collects data from:
- User actions and account information  
- Automatically collected device and usage data  
- Third-party sources (market data providers, banks, identity verification systems)

## Storage Layer
Two main storage layers are discussed:
- **Data Lake**: Stores raw market data, logs, and unprocessed events  
- **Data Warehouse**: Stores cleaned and structured data such as trading history, user profiles, and analytics tables  

## Processing Layer
Thndr utilizes both:
- **Batch Processing**: Daily portfolio calculations, market data cleaning, financial report generation  
- **Real-Time Processing**: Live stock price updates, instant order execution, in-app events  

## Serving Layer
Processed data is used for:
- **Dashboards**: Portfolio analytics, business monitoring, user activity tracking  
- **Machine Learning Models**: Fraud detection, user behavior insights, personalized recommendations  

## Thndr Abstracted Data Pipeline
A simplified view of the pipeline:

App + Market Feeds + Bank APIs  
↓  
Data Ingestion (Kafka)  
↓  
Data Lake (Raw Zone)  
↓  
Batch / Streaming Processing (Flink / Spark)  
↓  
Data Warehouse  
↓  
Dashboards – ML Models – Reporting

## References
- Thndr Privacy Policy  
- Thndr Blog  
- Deloitte Fintech Insights  

## Author
**Hassan Ashraf Hassan Al Sadaawy**  
DEPI – Data Engineering Track
