# Real-Time Transaction Streaming Pipeline (PoC)

Proof-of-concept for real-time streaming analytics on simulated financial transactions using PySpark Structured Streaming. Aligns with financial/IoT use cases for event ingestion, processing, and aggregation.

## Objective
Simulate high-volume transaction streams (e.g., debit/credit events), process in real-time, apply aggregations (windowed totals by type), and output for monitoring — demonstrating low-latency analytics without a full Kafka setup.

## Architecture Overview
- Event simulation → Rate source (mimics Kafka)
- Streaming ingestion → PySpark Structured Streaming
- Processing → Transformations, windowing, aggregations
- Output → Console sink (extendable to Delta Lake or dashboard)

## Tech Stack
- PySpark Structured Streaming
- Spark SQL
- Python

## Requirements
- pyspark==3.5.3

## Key Features & Outcomes
- Processed 10+ transactions per second in simulation
- Windowed aggregations (e.g., 1-minute totals by type)
- Real-time monitoring of counts and amounts
- Handles debit/credit types with status filtering

## Project Structure
-notebooks/                   # Main streaming notebook
-screenshots/                 # Visual results

## How to Run (Local PySpark or Databricks)
1. Install PySpark locally: `pip install pyspark.`
2. Open and run `notebooks/transaction_streaming_pipeline.ipynb.`
3. View console outputs (runs for 60 seconds)

Built by Ganesh Sai Ravuru  
Data Engineer | Multi-cloud Specialist
