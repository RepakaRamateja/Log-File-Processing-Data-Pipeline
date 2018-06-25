# Log-File-Processing-Data-Pipeline

Log file processing data pipeline built using Lambda architecture | Flume | Apache Spark | Spark Streaming | Apache Kafka | HDFS | Hbase | Hive | Impala | Oozie

</br>

## Introduction

Storing, processing and mining data from web server logs has become mainstream for a lot of companies today. Industry giants have used this engineering and the accompany science of machine learning to extract information that has helped in ads targeting, improved search, application optimization and general improvement in application's user experience.


</br>

## Goal

• In this hadoop project, we will be using a sample application log file from an application server to demonstrated a scaled-down server log processing pipeline. From ingestion to insight usually require Hadoop-ecosystem tools like Flume, Pig, Spark, Hive/Impala, Kafka, Oozie and HDFS for storage and this is what we will be looking at but holistically and specifically at each stage of the pipeline.

• However that processing was batch processing which operates in the batch and serving layer and in the lambda architecture(Batch, Speed, Serving),we also have speed layer. Now also going one step further by bringing processing to the speed layer of the lambda architecture which opens up more capabilities. One of such capability will be ability monitor application real time perform or measure real time comfort with applications or real time  alert in case of security breach.The abilities and functionalities will be explored using Spark Streaming in a streaming architecture. 

</br>

## Architecture

### High Level Architecture

![alt text](https://github.com/RepakaRamateja/Log-File-Processing-Data-Pipeline/blob/master/images/arch.jpeg)

</br>

### Batch layer

![alt text](https://github.com/RepakaRamateja/Log-File-Processing-Data-Pipeline/blob/master/images/batch.png)

 • Using Flume to ingest log data

 • Using Spark to process data

 • Integrating Kafka to complex event alert

 • Using Impala for the low-latency query of processed log data.

 • Coordinating the data processing pipeline with Oozie.


</br>

### Speed layer

![alt text](https://github.com/RepakaRamateja/Log-File-Processing-Data-Pipeline/blob/master/images/speed.png)

• Getting logs at real time using Flume Log4J appenders

• Custom Flume configuration for Spark Streaming

• Storing log event as a time series datasets in HBase

• Integrating Hive and HBase for data retrieval using query.

### Data Ingestion

![alt text](https://github.com/RepakaRamateja/Log-File-Processing-Data-Pipeline/blob/master/images/ingestion.png)

### Oozie Work flow

![alt text](https://github.com/RepakaRamateja/Log-File-Processing-Data-Pipeline/blob/master/images/oozie.png)


</br>

## Technology stack

  


