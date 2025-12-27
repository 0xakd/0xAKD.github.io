---
title: Big Data 101
tags: data-engineering
---

![cover](/images/big-data/Big-Data-Analytics.jpg)
## Overview
**Big Data** is about storing and processing very huge volume of data with the ultimate goal of generating insights from the data.

In the world of big data, data is processed either in batches or in real time. It's not just about the volume of data, it's also about the speed of data.

Traditional Databases are not designed to store, process and analyse this huge volume of data.

### 5 V's of Big Data
![5V's](/images/big-data/2023_04_5-vs-of-big-data.jpg)
1. **Volume:** It refers to the size of data that needs to be ingested into any Big Data solution. We measure data in bits (b), bytes (B), kilobytes (KB), megabytes (MB), gigabytes (GB), terabytes (TB), petabytes (PB), exabytes (EB), and so on. Depending on the volume, it is decided whether it is Big Data or not.
    * There is no official definition of big data in terms of size, As the total amount of available data grows exponentially every year.
    * Big Data refers to any datasets that are not manageable in a traditional way, with single cpu and storage.
2. **Velocity:** The speed at which the data is generated or enters into big data system. Big Data streams at a high velocity, often directly into memory rather than being stored in a disk.
    For example: there are millions of pictures/videos posted on instagram every minute.
3. **Variety:** It refers to the wide range of data formats.
Data might originates from multiple sources with distinct attributes. It can be:-
* **Structured** - In tabular format, grouped into rows and columns.
    eg.- csv or excel
* **Semi-structured** - Key-Value pairs that are stored into elements within a file.
    eg.- XML or JSON
* **Unstructured** - Everything else is unstructured data.
    eg.- images, texts, audio, etc.
4. **Veracity:** This refers to the truthfulness of the data. It is very important to ensure that the data is accurate for making the right decisions.
5. **Value:** The ability to extract meaningful and useful insights from the data to make it valuable.



## Storing Big Data 




### Distributed Storage
Rather than dumping all the data into a single machine, it is distributed to multiple machines, having their own CPU's and Memory, to enable parallel processing.<br>
Like this:
![distributed_storage](/images/big-data/Blank%20board.png)