# Log-File-Processing-Data-Pipeline

Log file processing data pipeline built using Lambda architecture | Flume | Apache Spark | Spark Streaming | Apache Kafka | HDFS | Hbase | Hive | Impala | Oozie

</br>

## Introduction

Storing, processing and mining data from web server logs has become mainstream for a lot of companies today. Industry giants have used this engineering and the accompany science of machine learning to extract information that has helped in ads targeting, improved search, application optimization and general improvement in application's user experience.

Lambda architecture is a data- processing architecture designed to handle massive quantities of data by taking advantage of both batch- and stream-processing methods.


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

![alt text](https://github.com/RepakaRamateja/Log-File-Processing-Data-Pipeline/blob/master/images/stack.png)

</br>    


<table>
<thead>
<tr>
<th>Area</th>
<th>Technology</th>
</tr>
</thead>
<tbody>
    <tr>
        <td> Data Ingestion tool </td>
        <td> Apache Flume </td>
    </tr>
    <tr>
        <td> Cluster Computing Framework </td>
        <td> Apache Spark and Spark Streaming (Scala)  </td>
    </tr>
    <tr>
        <td> Message Broker </td>
        <td> Apache Kafka </td>
    </tr>
    <tr>
        <td> Non-Relational Distributed Database </td>
        <td> Hbase </td>
    </tr>
    <tr>
        <td> Query Engine </td>
        <td> Hive and Impala </td>
    </tr>
    <tr>
        <td> Orchestration System for Batch Layer </td>
        <td> Oozie </td>
    </tr>
    <tr>
        <td> Distributed File System </td>
        <td> Hdfs </td>
    </tr>
</tbody>
</table>

</br>   

## Use Cases

Web Server Log Processing Use Case

• Application Health Monitoring

• Fraud - Security

• User Pattern (sessionizing a click stream) 

• User Experience

• Support Triage

• Metric Data Collection

</br>   

## Configuring Environment

</br>

  Download web server log dataset available from http://ita.ee.lbl.gov/html/contrib/NASA-HTTP.html, we must make analysis, event processing, and data retrieval of log data for varying kind possible.

Data from the log must be available either using low-latency querying tool or real-time event reporting and analysis.

Installation of Cloudera quickstart VM 5.7 or 5.8

Later Configuring Scala Runtime to Cloudera QuickStart VM

Watch the below video for more information 

https://www.youtube.com/watch?v=SFJsuo2XISs

</br>

</br>

## Execution Instructions

### Batch layer

please go through the files in batch/commands

flume_commands.txt

hdfs_command.txt

kafka_setup_run_command.txt

### Speed layer

please go through the file commands.txt in realtime

source code will be in spark streaming

## Screen shots
