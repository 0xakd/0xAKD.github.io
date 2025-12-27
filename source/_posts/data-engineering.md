---
title: What is Data Engineering?
tags: data-engineering
date: 2025-12-27 15:51:49
---


![cover](/images/data-engineering/What-is-Data-engineering.webp)
## What is Data Engineering??
Data Engineering is the practice of designing and building systems for the aggregation, storage, and processing of huge amount of data to make it available for downstream users.
<br>


### Key elements of data engineering
* **Data Extraction/collection:** Process of collecting raw data from various sources. This includes everything from structured data[in tabular format] to un-structured data[text, images, etc.].
* **Data Ingestion:** The process of transferring and loading Data into a target system in a reliable and repeated way.
* **Data Storage:** Data Engineers design the necessary storage solutions to _Store_ the Ingested data.
* **Data Transformation:** To make the data useful for data scientists, enabling them to perform their analysis.
* **Data Serving:** Once the data has been collected and processed, it's delivered to the end user.
<br>


### What do data engineers do?
Data Engineering involves many tasks, such as:
- Collecting data from various sources (apps, websites, etc.)
- Moving data to target destination.
- Storing unorganised raw data in a structured and organised manner.
- Validating and processing Big Data.
- Build data pipelines.
- Design Data storage systems.

<br>

### Data engineering vs Data Science vs Data analysis
**Data Engineers:** Data Engineers build and maintain data infrastructures to automate data ingestion, creation, storage and processing.<br>
**Data Scientists:** Data Scientists machine learning models, data exploration and other technologies to predict future outcomes. It is a very code heavy role like Data Engineering.<br>
**Data Analysts:** Data Analysts examine large datasets to identify trends and extract insights to help organisation make data-driven decisions. They work with predefined datasets.<br>


<br>

## Data Pipelines
![data_pipeline](/images/data-engineering/data_pipeline.png)
### What is a Data Pipeline
Data pipeline is a method in which raw data from various sources is ingested, transformed and then moved to a target destination, such as data lake or data warehouse, for analysis. 
<br>

### Types of Data Pipelines
There are mainly two types of Data Pipelines:
- **Batch data pipeline:** In Batch processing data pipeline, data is processed in large volumes or batches. It's often cost-efficient and mostly used for very large amount of data.

It performs a series of commands on every batch of data in sequence and gives output. after all the data processing is complete, it loads the entire batch into a cloud storage.
<br>

- **Streaming data pipeline:** Streaming data pipelines processes raw data almost instantly. It processes the data in real time as it is generated. It processes data even if some data packets are lost or delayed.

Streaming pipelines process a series of events for real-time analysis.
<br>
<br>

## Big Data Storage Systems
After data is processed, it must be stored in durable, secure, and scalable storage systems for future analysis and use.  
Two commonly used big data storage systems are data lakes and data warehouses.
<br>

### Data Lake 
Data lake is a storage repository which is designed to store a large amount of raw data that can be structured, semi-structured, and unstructured. Once the data reaches the data lake, it can be used for machine learning or training AI models.
<br>

### Data Warehouse
A Data Warehouse is an enterprise data platform, also called Enterprise Data Warehouse (EDW). It is used to aggregate data from various sources into a central database optimised for querying and analysis of the data.
A Data Warehouse can store both current and historical data in once place and is built to give a long-term insight over time.