# Programming Is Awesome
    
This is a collection of many frameworks and tools for software development.

Any **recommendations** and **suggestions** are welcomed.

## Table of Contents

- [Cloud Providers](#cloud-providers)
- [Big Data](#big-data)
    - [Big Data Distributor](#big-data-distributor)
    - [Big Data Ingestion Layer](#big-data-ingestion-layer)
    - [Big Data Speed Layer](#big-data-speed-layer)
    - [Big Data Batch Layer](#big-data-batch-layer)
    - [Resource Manager](#resource-manager)
    - [Distributed SQL Query Engine](#distributed-sql-query-engine)
    - [Machine Learning](#machine-learning)
    - [Notebook](#notebook)
- [Database](#database)
    - [Column Family](#column-family)
    - [Document Oriented](#document-oriented)
- [Data Warehouse](#data-warehouse)
- [Distributed File System](#distributed-file-system)
- [BI Tools](#bi-tools)   
- [Frameworks & Tools](#frameworks--tools)
    - [Reactive Framework](#reactive-framework)
    - [Micoservices Framework](#micoservices-framework)    
    - [Monitoring](#monitoring)
    - [Load Balancer](#load-balancer)
    - [API Gateway](#api-gateway)
    - [Testing Tools](#testing-tools)  
    - [Code Quality Analyzer](#code-quality-analyzer)  
    - [Code Security Analyzer](#code-security-analyzer)
    - [SQL Database Version Manager](#sql-database-version-manager)
    - [SMTP Server](#smtp-server)
- [Game Engines](#game-engines)

***********

## Cloud Providers
- [Amazon Web Services (AWS)](https://aws.amazon.com/) - Amazon Web Services offers reliable, scalable, and inexpensive cloud computing services. Free to join, pay only for what you use.
- [Microsoft Azure](https://azure.microsoft.com/) - Microsoft Azure is an open, flexible, enterprise-grade cloud computing platform.
- [Google Cloud Platform](https://cloud.google.com/) - Google Cloud Platform lets you build and host applications and websites, store data, and analyze data on Google's scalable infrastructure.
- [IBM Bluemix](https://www.ibm.com/cloud-computing/bluemix/) - Bluemix is an open standards, cloud platform for building, running, and managing apps and services.
- [OpenStack](https://www.openstack.org/) - OpenStack software controls large pools of compute, storage, and networking resources throughout a datacenter.
- [Apache CloudStack](https://cloudstack.apache.org/) - Apache CloudStack is open source software designed to deploy and manage large networks of virtual machines.
- [Cloud Foundry](https://www.cloudfoundry.org/) - Cloud Foundry is an open source cloud computing platform as a service (PaaS) originally developed by VMware and now overseen by the Cloud Foundry.
- [DigitalOcean](https://www.digitalocean.com/) - DigitalOcean is a simple and robust cloud computing platform, designed for developers. 
- [Heroku](https://www.heroku.com/) - Heroku is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud.

## Big Data

### Big Data Distributor
- [Amazon EMR](https://aws.amazon.com/emr/) - Amazon EMR simplifies big data processing, providing a managed Hadoop framework. 
- [Cloudera CDH](http://www.cloudera.com/) - CDH is Cloudera's software distribution containing Apache Hadoop and related projects. All components are 100% open source.
- [Hortonworks HDP](http://hortonworks.com/) - Hortonworks' product named Hortonworks Data Platform (HDP) includes Apache Hadoop and is used for storing, processing, and analyzing large volumes of data.
- [IBM BigInsights](http://www.ibm.com/analytics/us/en/technology/biginsights/) - IBM provides a complete solution of Hadoop, including Spark, to scale analytics quickly and easily. Available on-premises, on-cloud, and integrated with other systems in use today.
- [MapR](https://www.mapr.com/) - The MapR Converged Data Platform is the industry's only platform to integrate the enormous power of Hadoop and Spark with global event streaming, real-time.
- [Pivotal Big Data Suite](https://pivotal.io/big-data/pivotal-big-data-suite) - Pivotal Big Data Suite provides the flexibility to choose and adopt proven, open source, scale-out databases, including: Pivotal Greenplum, Pivotal HDB.
- [Databricks](https://databricks.com/) - Founded by the creators of Apache Spark, Databricks makes big data analytics simple through an integrated workspace hosted as a service in the cloud.
- [Concurrent](https://www.concurrent.com/) - One of the distributor in Hadoop world. 

### Big Data Ingestion Layer
- [Apache Kafka](https://kafka.apache.org/) - Kafka™ is used for building real-time data pipelines and streaming apps. 
- [Apache Flume](https://flume.apache.org/) - Flume is a distributed, reliable, and available service for efficiently collecting, aggregating, and moving large amounts of log data.
- [RabbitMQ](https://www.rabbitmq.com/) - RabbitMQ is open source message broker software that implements the Advanced Message Queuing Protocol (AMQP).
- [Mosquitto](https://mosquitto.org/) - Mosquitto is an open source message broker that implements the MQTT (MQ Telemetry Transport) protocol v3.1.
- [Logstash](https://www.elastic.co/products/logstash) - Logstash is an open source, server-side data processing pipeline that ingests data from a multitude of sources simultaneously.
- [Spring XD](http://projects.spring.io/spring-xd/) - Spring XD is a unified, distributed, and extensible service for data ingestion, real time analytics, batch processing, and data export.

### Big Data Speed Layer
- [Confluent Platform](http://www.confluent.io/) - The free, open-source streaming platform based on Apache Kafka. Confluent Platform is the best way to get started with real-time data streams.
- [Apache Storm](http://storm.apache.org/) - Apache Storm is a free and open source distributed realtime computation system.
- [Apache Spark Streaming](http://spark.apache.org/streaming/) - Spark Streaming brings Apache Spark's language-integrated API to stream processing, letting you write streaming jobs the same way you write batch jobs.
- [Apache Flume Interceptor](https://flume.apache.org/) - Flume is a distributed, reliable, and available service for efficiently collecting, aggregating, and moving large amounts of log data.
- [Apache Samza](http://samza.apache.org/) - Apache Samza is a distributed stream processing framework. It uses Apache Kafka for messaging, and Apache Hadoop YARN to provide fault tolerance.
- [Apache Gearpump](https://gearpump.apache.org/) - Apache Gearpump is a real-time big data streaming engine.
- [Spring XD](http://projects.spring.io/spring-xd/) - Spring XD is a unified, distributed, and extensible service for data ingestion, real time analytics, batch processing, and data export.

### Big Data Batch Layer
- [Apache Spark](http://spark.apache.org/) - Apache Spark™ is a fast and general engine for large-scale data processing.
- [Apache MapReduce](http://hadoop.apache.org/) - The Apache Hadoop MapReduce software library is a framework that allows for the distributed processing of large data sets across clusters of computers using simple programming models.
- [Spring XD](http://projects.spring.io/spring-xd/) - Spring XD is a unified, distributed, and extensible service for data ingestion, real time analytics, batch processing, and data export.
- [Apache Flink](https://flink.apache.org/) - Apache Flink® is an open source platform for distributed stream and batch data.

### Resource Manager
- [Apache Mesos](http://mesos.apache.org/) - Apache Mesos abstracts CPU, memory, storage, and other compute resources away from machines (physical or virtual), enabling fault-tolerant and elastic distributed systems to easily be built and run effectively.
- [Mesosphere](https://mesosphere.com/) - Mesosphere Enterprise DC/OS is an enterprise grade datacenter-scale operating system, providing a single platform for running containers, big data.
- [Apache Yarn](http://hadoop.apache.org/) - The Apache Hadoop Yarn software library is a framework that allows for the distributed processing of large data sets across clusters of computers using simple programming models.

### Distributed SQL Query Engine
- [Apache Impala](http://impala.apache.org/) - Apache Impala is the open source, native analytic database for Apache Hadoop. Impala is shipped by Cloudera, MapR, Oracle, and Amazon.
- [Apache Hive](https://hive.apache.org/) - Apache Hive is a data warehouse infrastructure built on top of Hadoop for providing data summarization, query, and analysis.
- [Spark SQL](http://spark.apache.org/sql/) - Spark SQL is a Spark module for structured data processing.
- [Apache Drill](https://drill.apache.org/) - Drill supports a variety of NoSQL databases and file systems, including HBase, MongoDB, MapR-DB, HDFS, MapR-FS, Amazon S3, Azure Blob Storage.
- [Presto](https://prestodb.io/) - Presto is an open source distributed SQL query engine for running interactive analytic queries against data sources of all sizes ranging.
- [Hive on Apache Tez](https://tez.apache.org/) - The Apache Tez™ project is aimed at building an application framework which allows for a complex directed-acyclic-graph of tasks for processing data.
- [Apache Phoenix](http://phoenix.apache.org/) - Apache Phoenix takes your SQL query, compiles it into a series of HBase scans.
- [Apache HAWQ](http://hawq.incubator.apache.org/) - Apache HAWQ (incubating) combines exceptional MPP-based analytics performance, robust ANSI SQL compliance, Hadoop ecosystem.
- [IBM Big SQL](http://www.ibm.com/analytics/us/en/technology/big-sql/) - IBM Big SQL is a data warehouse system for Hadoop that you use to summarize, query, and analyze data.
- [Apache Kylin](http://kylin.apache.org/) - Apache Kylin™ is an open source Distributed Analytics Engine.

### Machine Learning
- [Apache Mahout](https://mahout.apache.org/) - The Apache Mahout™ project's goal is to build an environment for quickly creating scalable performant machine learning applications.

### Notebook
- [Jupyter](http://jupyter.org/) - Open source, interactive data science and scientific computing across over 40 programming languages.

<br>

## Database

### Column Family
- [DataStax Enterprise](http://www.datastax.com/) - DataStax powers the big data applications that transform business and profoundly improve customer experiences through Apache Cassandra™.
- [Amazon DynamoDB](https://aws.amazon.com/documentation/dynamodb/) - Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability.
- [Cassandra](http://cassandra.apache.org/) - The Apache Cassandra database is the right choice when you need scalability and high availability without compromising performance.
- [Apache HBase](http://hbase.apache.org/) - Apache HBase™ is the Hadoop database, a distributed, scalable, big data store. Use Apache HBase™ when you need random, realtime read/write access.
- [Apache Accumulo](https://accumulo.apache.org/) - Apache Accumulo™ is a sorted, distributed key/value store that provides robust, scalable data storage and retrieval.
- [Riak KV](http://basho.com/products/riak-kv/) - Riak® KV is a distributed NoSQL key-value database with advanced local and multi-cluster replication that guarantees reads and writes even in the event of hardware failures or network partitions.

### Document Oriented
- [MongoDB](https://www.mongodb.com/) - MongoDB for GIANT Ideas - Build innovative modern applications that create a competitive advantage.

<br>

## Data Warehouse
- [Redshift](https://aws.amazon.com/documentation/redshift/) - Amazon Redshift is a fast, fully managed, petabyte-scale data warehouse service.

<br>

## Distributed File System
- [DSEFS](https://docs.datastax.com/en/latest-dse/datastax_enterprise/ana/aboutDsefs.html) - DSEFS (DataStax Enterprise file system) is a new distributed file system within DataStax Enterprise.

<br>

## BI Tools
- [Tableau](https://www.tableau.com/) - Tableau is data visualization software.

<br>

## Frameworks & Tools

### Reactive Framework
- [Akka](http://akka.io/) - Akka is a toolkit and runtime for building highly concurrent, distributed, and resilient message-driven applications on the JVM.

### Micoservices Framework
- [Lagom](http://www.lagomframework.com/) - Lagom is a framework for creating reactive microservice-based systems.

### Monitoring
- [Ganglia](http://ganglia.info/) - Ganglia is a scalable distributed monitoring system for high-performance computing systems such as clusters and Grids.

### Load Balancer
- [HAProxy](http://www.haproxy.org/) - The Reliable, High Performance TCP/HTTP Load Balancer.

### API Gateway
- [Tyk](https://tyk.io/) - Tyk is an open source API Gateway that is fast, scalable and modern.
- [WSO2](http://wso2.com/) - WSO2 provides the open source enterprise platform that helps to build, integrate, analyse and manage your APIs, applications, and Web services.

### Testing Tools
- [JUnit](http://junit.org/) - JUnit is a simple framework to write repeatable tests.

### Code Quality Analyzer
- [SonarQube](http://www.sonarqube.org/) - SonarQube is an open platform to manage code quality.

### Code Security Analyzer
- [Checkmarx](https://www.checkmarx.com/) - Checkmarx is a provider of state-of-the-art application security solution: static code analysis software, seamlessly integrated into development process.

### SQL Database Version Manager
- [Flyway](https://flywaydb.org/) - Flyway lets you regain control of your database migrations with pleasure and plain sql.

### SMTP Server
- [Apache James](https://james.apache.org/) - The Apache Java Mail Server is a 100% pure Java SMTP, IMAP4 and POP3 Mail server designed to be a complete and portable enterprise mail. 

<br>

## Game Engines
- [Unity3D](https://unity3d.com/) - Unity3D is a cross-platform game engine developed by Unity Technologies and used to develop video games for PC, consoles, mobile devices and websites.

**[⬆ back to top](#table-of-contents)**

