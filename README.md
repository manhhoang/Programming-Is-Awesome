# Programming Is Awesome

This is a collection of many frameworks and tools for software development.

Any **recommendations** and **suggestions** are welcomed.

## Table of Contents

- [Architecture](#architecture)
- [Programming Languages](#programming-languages)
- [Algorithms](#algorithms)
    - [Algorithm Techniques](#algorithm-techniques)    
    - [Algorithm Fundamental](#algorithm-fundamental)
    - [Data Structures](#data-structures)
- [Parallel Programming](#parallel-programming)
- [Cloud Providers](#cloud-providers)
- [Data Science](#data-science)
    - [Machine Learning](#machine-learning)
    - [Deep Learning](#deep-learning)
    - [ML Tools](#ml-tools)
    - [Notebook](#notebook)
    - [AI Tools](#ai-tools)
- [Frameworks & Tools](#frameworks--tools)
    - [Reactive Framework](#reactive-framework)
    - [Micoservices Framework](#micoservices-framework)
    - [ORM](#orm)
    - [Monitoring](#monitoring)
    - [Load Balancer](#load-balancer)
    - [API Gateway](#api-gateway)
    - [Testing Tools](#testing-tools)  
    - [Code Quality Analyzer](#code-quality-analyzer)  
    - [Code Security Analyzer](#code-security-analyzer)
    - [SQL Database Version Manager](#sql-database-version-manager)
    - [SMTP Server](#smtp-server)
    - [Profiling Tools](#profiling-tools)
    - [Distributed Job Scheduler](#distributed-job-scheduler)
- [Database](#database)
    - [Database Indexing](#database-indexing)
    - [Column Family](#column-family)
    - [Document Oriented](#document-oriented)
    - [Search DB](#search-db)
    - [Graph DB](#graph-db)
    - [NewSQL](#newsql)
    - [In-memory DB](#in-memory-db)
    - [Event Store](#event-store)
    - [Embedded Database](#embedded-database)
    - [Time Series](#time-series)
- [Data Warehouse](#data-warehouse)
- [Storage](#storage)
- [Blockchain](#blockchain)
- [Big Data](#big-data)
    - [Big Data Distributor](#big-data-distributor)
    - [Big Data Ingestion Layer](#big-data-ingestion-layer)
    - [Big Data Speed Layer](#big-data-speed-layer)
    - [Big Data Batch Layer](#big-data-batch-layer)
    - [Resource Manager](#resource-manager)
    - [Distributed SQL Query Engine](#distributed-sql-query-engine)        
- [Distributed File System](#distributed-file-system)
- [BI Tools](#bi-tools)   
- [DevOps](#devops)
- [Security](#security)
- [Web Frameworks](#web-frameworks)
- [Mobile Frameworks](#mobile-frameworks)
- [Game Engines](#game-engines)
- [IoT](#iot)
    - [IoT OS](#iot-os)
- [UML Tools](#uml-tools)     
- [Summit Events](#summit-events)

***********

## Architecture
![ScreenShot](https://dl.dropboxusercontent.com/u/974078/Architecture.png)

- [SMACK Stack](http://www.cakesolutions.net/teamblogs/smack-stack-on-dcos) - The SMACK stack consists of Spark, Mesos, Akka, Cassandra and Kafka.
- [Functional programming](https://en.wikipedia.org/wiki/Functional_programming) - Functional programming is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data. 
- [Microservices](https://en.wikipedia.org/wiki/Microservices) - Microservices is a specialisation of and implementation approach for distributed architectures used to build flexible, independently deployable software systems.

![Alt text](resources/Microservices_architecture.PNG?raw=true)

  **Kafka is the data pipelines for the organisation data. Both synchronous and asynchronous communication strategies have their use, 
  but you should make an effort to architect your system of microservices using asynchronous communication whenever possible.**
    
- [Reactive Programming](https://en.wikipedia.org/wiki/Reactive_programming) - Reactive programming is about non-blocking applications that are asynchronous and event-driven and require a small number of threads to scale.
- [Lambda Architecture](http://lambda-architecture.net/) - Lambda architecture is a data-processing architecture designed to handle massive quantities of data by taking advantage of both batch- and stream-processing.
- [CQRS](http://martinfowler.com/bliki/CQRS.html) - Command and Query Responsibility Segregation (CQRS) is a pattern that segregates the operations that read data (Queries) from the operations that update data (Commands) by using separate interfaces.
- [Event Sourcing](http://microservices.io/patterns/data/event-sourcing.html) - Event Sourcing persists each business entity as a sequence of events, and events are immutable.
- [Materialized View](https://en.wikipedia.org/wiki/Materialized_view) - A materialized view is a database object that contains the results of a query.
- [DDD](https://en.wikipedia.org/wiki/Domain-driven_design) - Domain-driven design (DDD) is an approach to software development for complex needs by connecting the implementation to an evolving model.

***********

## Programming Languages
- [Java](https://docs.oracle.com/javase/tutorial/) - Java is a general-purpose computer programming language that is concurrent, class-based, object-oriented.
![Alt text](resources/Java_collection_cheat_sheet.PNG?raw=true)
- [Scala](http://www.scala-lang.org/) - General purpose language; multiparadigm (object-oriented, functional, concurrent elements); statically typed, type-safe; focus: Web services.
![Alt text](resources/Scala_collections_cheat_sheet.png?raw=true)
- [Go](https://golang.org/) - Go is an open source programming language that makes it easy to build simple, reliable, and efficient software.
- [Python](https://www.python.org/) - Python is a widely used high-level, general-purpose, interpreted, dynamic programming language.
- [JavaScript](https://en.wikipedia.org/wiki/JavaScript) - JavaScript is a high-level, dynamic, untyped, and interpreted programming language. It has been standardized in the ECMAScript language specification.

***********

## Algorithms

### Algorithm Techniques
- [Two Pointer](https://tp-iiita.quora.com/The-Two-Pointer-Algorithm) -  The legendary two pointer approach is one such technique which is less of a talk and more of a discussion on the problems.
- [Dynamic Programming](https://en.wikipedia.org/wiki/Dynamic_programming) - Dynamic programming (also known as dynamic optimization) is a method for solving a complex problem by breaking it down into a collection of simpler subproblems, solving each of those subproblems just once, and storing their solutions.
- [Greedy](https://en.wikipedia.org/wiki/Greedy_algorithm) - Greedy algorithm is an algorithmic paradigm that follows the problem solving heuristic of making the locally optimal choice at each stage with the hope of finding a global optimum.
- [Backtracking](https://en.wikipedia.org/wiki/Backtracking) - Backtracking is a general algorithm for finding all (or some) solutions to some computational problems.
- [Brute Force](http://faculty.simpson.edu/lydia.sinapova/www/cmsc250/LN250_Levitin/L05-BruteForce.htm) - Brute force is a straightforward approach to solve a problem based on the problem’s statement and definitions of the concepts involved.

### Algorithm Fundamental
- [Sorting](http://algs4.cs.princeton.edu/20sorting/) - Sorting is the process of rearranging a sequence of objects so as to put them in some logical order.
![Alt text](resources/Sorting_algorithm_cheat_sheet.PNG?raw=true)

###### Selection Sort
```
    public int[] sort(int[] arr) {
        for (int i = 0; i < arr.length - 1; i++) {
            int index = i;
            for (int j = i + 1; j < arr.length; j++) {
                if (arr[j] < arr[index])
                    index = j;
            }
            int temp = arr[index];
            arr[index] = arr[i];
            arr[i] = temp;
        }
        return arr;
    }
```
    
###### Insertion Sort - Stable               
```
    public void sort(int[] a) {
        int temp;
        for (int i = 1; i < a.length; i++) {
            for (int j = i; j > 0; j--) {
                if (a[j] < a[j - 1]) {
                    temp = a[j];
                    a[j] = a[j - 1];
                    a[j - 1] = temp;
                }
            }
        }
    }
```

###### Bubble Sort - Stable
```
    public void sort(int[] a) {
        int j;
        boolean flag = true;
        int temp;   //holding variable

        while (flag) {
            flag = false;
            for (j = 0; j < a.length - 1; j++) {
                if (a[j] > a[j + 1]) { 
                    temp = a[j];               
                    a[j] = a[j + 1];
                    a[j + 1] = temp;
                    flag = true; 
                }
            }
        }
    }
```

###### Merge Sort - Stable
```
    public Comparable[] mergeSort(Comparable[] list) {
        if (list.length <= 1) {
            return list;
        }

        Comparable[] first = new Comparable[list.length / 2];
        Comparable[] second = new Comparable[list.length - first.length];
        System.arraycopy(list, 0, first, 0, first.length);
        System.arraycopy(list, first.length, second, 0, second.length);

        mergeSort(first);
        mergeSort(second);

        merge(first, second, list);
        return list;
    }

    private void merge(Comparable[] first, Comparable[] second, Comparable[] result) {
        int iFirst = 0;
        int iSecond = 0;
        int iMerged = 0;
        while (iFirst < first.length && iSecond < second.length) {
            if (first[iFirst].compareTo(second[iSecond]) < 0) {
                result[iMerged] = first[iFirst];
                iFirst++;
            } else {
                result[iMerged] = second[iSecond];
                iSecond++;
            }
            iMerged++;
        }
        System.arraycopy(first, iFirst, result, iMerged, first.length - iFirst);
        System.arraycopy(second, iSecond, result, iMerged, second.length - iSecond);
    }
```

###### Quick Sort
```
    public void quickSort(int[] arr, int low, int high) {
        if (arr == null || arr.length == 0)
            return;

        if (low >= high)
            return;

        // pick the pivot
        int middle = low + (high - low) / 2;
        int pivot = arr[middle];

        int i = low, j = high;
        while (i <= j) {
            while (arr[i] < pivot) {
                i++;
            }

            while (arr[j] > pivot) {
                j--;
            }

            if (i <= j) {
                int temp = arr[i];
                arr[i] = arr[j];
                arr[j] = temp;
                i++;
                j--;
            }
        }

        if (low < j)
            quickSort(arr, low, j);

        if (high > i)
            quickSort(arr, i, high);
    }
```
###### Radix Sort
```
    private int getMax(int arr[], int n) {
        int mx = arr[0];
        for (int i = 1; i < n; i++)
            if (arr[i] > mx)
                mx = arr[i];
        return mx;
    }

    private void countingSort(int arr[], int n, int exp) {
        int output[] = new int[n];
        int i;
        int count[] = new int[10];
        Arrays.fill(count, 0);

        for (i = 0; i < n; i++)
            count[(arr[i] / exp) % 10]++;

        for (i = 1; i < 10; i++)
            count[i] += count[i - 1];

        for (i = n - 1; i >= 0; i--) {
            output[count[(arr[i] / exp) % 10] - 1] = arr[i];
            count[(arr[i] / exp) % 10]--;
        }

        for (i = 0; i < n; i++)
            arr[i] = output[i];
    }

    public void radixsort(int arr[], int n) {
        // Find the maximum number to know number of digits
        int m = getMax(arr, n);

        for (int exp = 1; m / exp > 0; exp *= 10)
            countingSort(arr, n, exp);
    }
```

- [Searching](http://algs4.cs.princeton.edu/30searching/) - Modern computing and the internet have made accessible a vast amount of information.
###### Binary Search
```
    public int binarySearch(int key, int[] a) {
        Arrays.sort(a);
        int low = 0;
        int high = a.length - 1;
        while (low <= high) {
            int middle = (low + high) / 2;
            if (a[middle] == key) {
                return a[middle];
            }
            if (a[middle] < key) {
                low = middle + 1;
            }
            if (a[middle] > key) {
                high = middle - 1;
            }
        }
        return -1;
    }
```
###### Depth First Search
```
    private final int ROW = 5, COL = 5;

    private int dfs(int m[][], int i, int j, boolean visited[][]) {
        // These arrays are used to get row and column numbers of 8 neighbors of a given cell
        int x[] = new int[] {-1, -1, -1,  0, 0,  1, 1, 1};
        int y[] = new int[] {-1,  0,  1, -1, 1, -1, 0, 1};
        int no = 1;
        visited[i][j] = true;

        // Recur for all connected neighbours
        for (int k = 0; k < 8; ++k){
            int a = i + x[k];
            int b = j + y[k];
            if (a >= 0 && a < ROW && b >= 0 && b < COL && m[a][b]==1 && !visited[a][b]){
                int c = dfs(m, a, b, visited);
                no += c;
            }
        }
        return no;
    }
```
###### Breadth First Search
```
    private final int ROW = 5, COL = 5;

    public int[][] bfs(int[][] map, Point start){
        int[] x = {0,  0, 1, -1}; //This represent 4 directions right, left, down , up
        int[] y = {1, -1, 0,  0}; //This represent 4 directions right, left, down , up
        LinkedList<Point> q = new LinkedList<>();
        q.add(start);
        boolean[][] visited = new boolean[COL][ROW];
        for(boolean[] v : visited){
            Arrays.fill(v, false);
        }
        int[][] distTo = new int[COL][ROW];
        distTo[start.x][start.y] = 0;
        visited[start.x][start.y] = true;
        while(!q.isEmpty()){
            Point p = q.removeFirst();
            for(int i = 0; i < 4; i++){
                int a = p.x + x[i];
                int b = p.y + y[i];
                if(a >= 0 && b >= 0 && a < ROW && b < COL && !visited[a][b] && map[a][b] == 0){
                    distTo[a][b] = distTo[p.x][p.y] + 1;
                    visited[a][b] = true;
                    q.add(new Point(a,b));
                }
            }
        }

        return distTo;
    }
```
    
- [String](http://algs4.cs.princeton.edu/50strings/) - We communicate by exchanging strings of characters. We consider classic algorithms for addressing the underlying computational challenges surrounding applications.
- [Graph](http://algs4.cs.princeton.edu/40graphs/) - Typical graph algorithm problems for this example would be to determine how two people are related, or to draw this graph as a nice picture of the family tree.

### Data Structures
![Alt text](resources/Datastructure_cheat_sheet.PNG?raw=true)
- [LinkedList](http://www.geeksforgeeks.org/data-structures/#LinkedList) - Like arrays, Linked List is a linear data structure. Unlike arrays, linked list elements are not stored at contiguous location; the elements are linked using pointers.
- [Stack](http://www.geeksforgeeks.org/stack/) - A stack is an abstract data type that serves as a collection of elements, with two principal operations: push, which adds an element to the collection, and pop, which removes the most recently added element that was not yet removed.
- [Queue](http://www.geeksforgeeks.org/data-structures/#Queue) - Queue is an abstract data structure, somewhat similar to Stacks. Unlike stacks, a queue is open at both its ends. One end is always used to insert data (enqueue) and the other is used to remove data (dequeue).
- [Binary Tree](http://www.geeksforgeeks.org/binary-tree-2/) - A binary tree is a tree data structure in which each node has at most two children, which are referred to as the left child and the right child.
- [Binary Search Tree](http://www.geeksforgeeks.org/data-structures/#BinarySearchTree) - A Binary Search Tree (BST) is a tree in which all the nodes follow the below-mentioned properties − The left sub-tree of a node has a key less than or equal to its parent node's key. The right sub-tree of a node has a key greater than or equal to its parent node's key.
- [Red-Black Tree](http://www.geeksforgeeks.org/red-black-tree-set-1-introduction-2/) - Red-Black Tree is a self-balancing Binary Search Tree (BST).
- [Binary Heap](http://www.geeksforgeeks.org/heap/) - A binary heap is a complete binary tree which satisfies the heap ordering property. The ordering can be one of two types: the min-heap property: the value of each node is greater than or equal to the value of its parent, with the minimum-value element at the root.
- [Trie](http://www.geeksforgeeks.org/data-structures/#AdvancedDataStructure) - A trie, also called digital tree and sometimes radix tree or prefix tree (as they can be searched by prefixes), is a kind of search tree—an ordered tree data structure that is used to store a dynamic set or associative array where the keys are usually strings.
- [Suffix Tree](http://www.geeksforgeeks.org/data-structures/#AdvancedDataStructure) - A suffix tree (also called PAT tree or, in an earlier form, position tree) is a compressed trie containing all the suffixes of the given text as their keys and positions in the text as their values.
- [Inverted Index](https://en.wikipedia.org/wiki/Inverted_index) - In computer science, an inverted index (also referred to as postings file or inverted file) is an index data structure storing a mapping from content, such as words or numbers, to its locations in a database file, or in a document or a set of documents.

***********

## Parallel Programming
- [Actor Model](https://en.wikipedia.org/wiki/Actor_model) - The actor model in computer science is a mathematical model of concurrent computation that treats "actors" as the universal primitives of concurrent computation.
- [Communicating sequential processes](https://en.wikipedia.org/wiki/Communicating_sequential_processes) - Communicating sequential processes (CSP) is a formal language for describing patterns of interaction in concurrent systems. It is a member of the family of mathematical theories of concurrency known as process algebras, or process calculi, based on message passing via channels.

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
- [SAP HANA Cloud Platform](https://hcp.sap.com/index.html) - SAP HANA Cloud Platform is an open platform-as-a-service that provides unique in-memory database and application services.
- [Oracle Cloud](https://cloud.oracle.com/) - Oracle Cloud Platform as a Service (PaaS) helps enterprise IT and independent software vendor (ISV) developers rapidly build and deploy rich applications.

***********

## Data Science

### Machine Learning
- [Scikit Learn](http://scikit-learn.org/stable/) - An open source Python library that implements a range of machine learning, preprocessing, cross-validation and visualization algorithms.
- [Apache Mahout](https://mahout.apache.org/) - The Apache Mahout™ project's goal is to build an environment for quickly creating scalable performant machine learning applications.
- [Spark MLlib](http://spark.apache.org/mllib/) - MLlib is Apache Spark's scalable machine learning library.
- [H2O](http://www.h2o.ai/) - H2O is open-source software for big-data analysis.
- [Apache MADlib](https://madlib.incubator.apache.org/) - Apache MADlib (incubating): Big Data Machine Learning in SQL.
- [Weka](http://www.cs.waikato.ac.nz/ml/weka/) - Waikato Environment for Knowledge Analysis (Weka) is a popular suite of machine learning software written in Java, developed at the University of Waikato.
- [Apache SystemML](https://systemml.apache.org/) - Apache SystemML provides an optimal workplace for Machine Learning using big data.
- [SAS Enterprise Miner](https://www.sas.com/en_us/software/enterprise-miner.html) - SAS Enterprise Miner is a solution to create accurate predictive and descriptive models on large volumes of data across different sources in the organization.
- [IBM SPSS Modeler](http://www-03.ibm.com/software/products/en/spss-modeler) - IBM SPSS Modeler is a data mining and text analytics software application from IBM. It is used to build predictive models and conduct other analytic tasks.

### Deep Learning
- [TensorFlow](https://www.tensorflow.org/) - TensorFlow™ is an open source software library for numerical computation using data flow graphs.
- [Theano](http://deeplearning.net/software/theano/) - Theano is a Python library that allows you to define, optimize, and evaluate mathematical expressions involving multi-dimensional arrays efficiently.
- [Caffe](http://caffe.berkeleyvision.org/) - Caffe is a deep learning framework made with expression, speed, and modularity.
- [Torch](http://torch.ch/) - Torch is a scientific computing framework with wide support for machine learning algorithms that puts GPUs first.
- [OpenNLP](https://opennlp.apache.org/) - Apache OpenNLP is a Java machine learning toolkit for natural language processing (NLP).

### ML Tools
- [Numpy](http://www.numpy.org/) - NumPy is the fundamental package for scientific computing with Python. It contains among other things: a powerful N-dimensional array object.
- [SciPy](https://www.scipy.org/) - Open Source Library of Scientific Tools. SciPy supplements the popular Numeric module, gathering a variety of high level science and engineering modules.
- [Pandas](http://pandas.pydata.org/) - Pandas is an open source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming.
- [Matplotlib](http://matplotlib.org/) - 2D plotting library which produces publication quality figures in a variety of hardcopy formats and interactive environments across platforms.
- [PyData](http://pydata.org/) - PyData is a gathering of users and developers of data analysis tools in Python.
- [R](https://www.r-project.org/) - R, also called GNU S, is a strongly functional language and environment to statistically explore data sets, make many graphical displays of data.

### Notebook
- [Jupyter](http://jupyter.org/) - Open source, interactive data science and scientific computing across over 40 programming languages.
- [Zeppelin](https://zeppelin.apache.org/) - Apache Zeppelin interpreter concept allows any language/data-processing-backend to be plugged into Zeppelin.
- [RStudio](https://www.rstudio.com/) - A powerful and productive user interface for R.

### AI Tools
- [IBM Data Science Experience](http://datascience.ibm.com/) - IBM Data Science Experience is an interactive, collaborative, cloud-based environment where data scientists can use multiple tools.
- [IBM Watson](http://www.ibm.com/watson/) - IBM Watson is a technology platform that uses natural language processing and machine learning to reveal insights from large amounts of unstructured data.
- [OpenCV](http://opencv.org/) - OpenCV (Open Source Computer Vision) is a library of programming functions mainly aimed at real-time computer vision.

***********

## Frameworks & Tools

### Reactive Framework
- [Akka](http://akka.io/) - Akka is a toolkit and runtime for building highly concurrent, distributed, and resilient message-driven applications on the JVM.
- [Reactor](http://projectreactor.io/) - Reactor is a fully non-blocking foundation with efficient demand management.
- [ReactiveX](http://reactivex.io/) - ReactiveX is a combination of the best ideas from the Observer pattern, the Iterator pattern, and functional programming.
- [Erlang](https://www.erlang.org/) - Erlang is a programming language used to build massively scalable soft real-time systems with requirements on high availability.
- [Goroutines](https://gobyexample.com/goroutines) - A goroutine is a function that is capable of running concurrently with other functions.
- [Vert.x](http://vertx.io/) - Vert.x is a tool-kit for building reactive applications on the JVM.
- [Play Framework](https://www.playframework.com/) - Play Framework makes it easy to build web applications with Java & Scala. Play is based on a lightweight, stateless, web-friendly architecture. Built on Akka.
- [Spring Web Reactive](http://docs.spring.io/spring-framework/docs/5.0.0.M1/spring-framework-reference/html/web-reactive.html) - Reactive programming is about non-blocking applications that are asynchronous and event-driven and require a small number of threads to scale.

### Micoservices Framework
- [Akka HTTP](https://github.com/akka/akka-http) - The Akka HTTP modules implement a full server- and client-side HTTP stack on top of akka-actor and akka-stream. It's not a web-framework but rather a more general toolkit for providing and consuming HTTP-based services.
- [Lagom](http://www.lagomframework.com/) - Lagom is a framework for creating reactive microservice-based systems.
- [Play Framework](https://www.playframework.com/) - Play Framework makes it easy to build web applications with Java & Scala. Play is based on a lightweight, stateless, web-friendly architecture. Built on Akka.
- [Spring Boot](https://projects.spring.io/spring-boot/) - Spring Boot makes it easy to create stand-alone, production-grade Spring based Applications that you can "just run".
- [Dropwizard](http://www.dropwizard.io/) - Dropwizard is a Java framework for developing ops-friendly, high-performance, RESTful web services.
- [Sparkjava](http://sparkjava.com/) - Spark Framework - Create web applications in Java rapidly. Spark is a micro web framework that lets you focus on writing your code, not boilerplate code.
- [Gin](https://github.com/gin-gonic/gin) - Gin is a web framework written in Go (Golang). It features a martini-like API with much better performance, up to 40 times faster thanks to httprouter.

### ORM
- [Hibernate](http://hibernate.org/) - Hibernate an open source Java persistence framework project.
- [JPA](https://en.wikipedia.org/wiki/Java_Persistence_API) - The Java Persistence API (JPA) is a Java application programming interface specification that describes the management of relational data in applications using Java Platform.
- [EclipseLink](http://www.eclipse.org/eclipselink/) - The software provides an extensible framework that allows Java developers to interact with various data services, including databases, web services, Object XML mapping (OXM), and Enterprise Information Systems (EIS).
- [Slick](http://slick.lightbend.com/) - Slick is a modern database query and access library for Scala. 

### Monitoring
- [Ganglia](http://ganglia.info/) - Ganglia is a scalable distributed monitoring system for high-performance computing systems such as clusters and Grids.
- [Nagios](https://www.nagios.org/) - Nagios provides enterprise-class Open Source IT monitoring, network monitoring, server and applications monitoring.
- [Datadog](https://www.datadoghq.com/) - See metrics from all of your apps, tools & services in one place with Datadog's cloud monitoring as a service solution.
- [New Relic](https://newrelic.com/) - A software analytics tool suite used by developers, ops, and software companies to understand how your applications are performing in development.
- [Perfino](https://www.ej-technologies.com/products/perfino/overview.html) - Perfino is a zero-overhead APM solution for monitoring Java application servers.
- [Sensu](https://sensuapp.org/) - Monitor servers, services, application health, and business KPIs.
- [OverOps](https://www.overops.com/) - Know why Java code fails in production.

### Load Balancer
- [HAProxy](http://www.haproxy.org/) - The Reliable, High Performance TCP/HTTP Load Balancer.
- [Marathon-LB](https://github.com/mesosphere/marathon-lb) - Marathon-lb is a tool for managing HAProxy, by consuming Marathon's app state.

### API Gateway
- [Tyk](https://tyk.io/) - Tyk is an open source API Gateway that is fast, scalable and modern.
- [WSO2](http://wso2.com/) - WSO2 provides the open source enterprise platform that helps to build, integrate, analyse and manage your APIs, applications, and Web services.

### Testing Tools
- [JUnit](http://junit.org/) - JUnit is a simple framework to write repeatable tests.
- [Mockito](http://site.mockito.org/) - A mocking framework for unit tests written in Java.
- [TestNG](http://testng.org/) - TestNG is a testing framework developed in the lines of JUnit and NUnit.
- [DbUnit](http://dbunit.sourceforge.net/) - A JUnit extension that puts a database into a known state between test runs.
- [Selenium](http://docs.seleniumhq.org/) - Selenium is a suite of tools to automate web browsers across many platforms.
- [Cucumber](https://cucumber.io/) - Cucumber is a software tool that computer programmers use for testing other software.
- [SoapUI](https://www.soapui.org/) - SoapUI, is the world leading Open Source Functional Testing tool for API Testing.
- [LoadUI](https://www.loadui.org/) - LoadUI, a Performance Load Testing tool for APIs & Web Services.
- [Secure Pro](https://smartbear.com/product/ready-api/secure/overview/) - Simulate attacks against your REST and SOAP services so you know they're safe. Build a Trusted API with Secure Pro, Based on The world's Most Trusted API.

### Code Quality Analyzer
- [SonarQube](http://www.sonarqube.org/) - SonarQube is an open platform to manage code quality.
- [Gerrit](https://www.gerritcodereview.com/) - Gerrit provides web based code review and repository management for the Git version control system.
- [PMD](https://pmd.github.io/) - PMD is a source code analyzer.

### Code Security Analyzer
- [Checkmarx](https://www.checkmarx.com/) - Checkmarx is a provider of state-of-the-art application security solution: static code analysis software, seamlessly integrated into development process.

### SQL Database Version Manager
- [Flyway](https://flywaydb.org/) - Flyway lets you regain control of your database migrations with pleasure and plain sql.
- [Liquibase](http://www.liquibase.org/) - Liquibase is an open source database-independent library for tracking, managing and applying database schema changes. 
- [RedGate](http://www.red-gate.com/) - Redgate's DLM(Database Lifecycle Management) solution helps you put in place a trusted, scalable and repeatable database change management process.

### SMTP Server
- [Apache James](https://james.apache.org/) - The Apache Java Mail Server is a 100% pure Java SMTP, IMAP4 and POP3 Mail server designed to be a complete and portable enterprise mail. 

### Profiling Tools
- [JProfiler](https://www.ej-technologies.com/products/jprofiler/overview.html) - JProfiler is the leading Java Profiler for profiling on the JVM.
 
### Distributed Job Scheduler
- [Quartz](http://www.quartz-scheduler.org/) - Quartz is a job scheduling library that can be integrated into a wide variety of Java applications.
- [Celery](http://www.celeryproject.org/) - Celery is a simple, flexible, and reliable distributed system to process vast amounts of messages.

***********

## Database

### Database Indexing

- **Hash Index** - They are used only for equality comparisons that use the = operators (but are very fast). 
They are not used for comparison operators such as < that find a range of values. Systems that rely on this type of single-value lookup are known as “key-value stores”.
Only whole keys can be used to search for a row. (With a B-tree index, any leftmost prefix of the key can be used to find rows.)
- **Bitmap Index** - Bitmap indexes are not suitable for OLTP applications with large numbers of concurrent transactions modifying the data. 
These indexes are primarily intended for decision support (DSS) in data warehousing applications where users typically query the data rather than update it.
The advantages of using bitmap indexes are greatest for low cardinality columns: that is, columns in which the number of distinct values is small compared to the number of rows in the table. 
A gender column, which only has two distinct values (male and female), is ideal for a bitmap index.
Data is frequently updated in and deleted from OLTP applications, bitmap indexes can cause a serious locking problem in these situations.
- **B-tree Index** - A B-tree index can be used for column comparisons in expressions that use the =, >, >=, <, <=, or BETWEEN operators. 
The index also can be used for LIKE comparisons if the argument to LIKE is a constant string that does not start with a wildcard character.
B-tree indexes are well suited for OLTP applications in which users' queries are relatively routine.
- **Inverted Index** - This type of index is called an inverted index, because it inverts a page-centric data structure (page->words) to a keyword-centric data structure (word->pages).

### Column Family
- [DataStax Enterprise](http://www.datastax.com/) - DataStax powers the big data applications that transform business and profoundly improve customer experiences through Apache Cassandra™.
- [Amazon DynamoDB](https://aws.amazon.com/documentation/dynamodb/) - Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability.
- [Cassandra](http://cassandra.apache.org/) - The Apache Cassandra database is the right choice when you need scalability and high availability without compromising performance.
- [Apache HBase](http://hbase.apache.org/) - Apache HBase™ is the Hadoop database, a distributed, scalable, big data store. Use Apache HBase™ when you need random, realtime read/write access.
- [Apache Accumulo](https://accumulo.apache.org/) - Apache Accumulo™ is a sorted, distributed key/value store that provides robust, scalable data storage and retrieval.
- [Riak KV](http://basho.com/products/riak-kv/) - Riak® KV is a distributed NoSQL key-value database with advanced local and multi-cluster replication that guarantees reads and writes even in the event of hardware failures or network partitions.

### Document Oriented
- [MongoDB](https://www.mongodb.com/) - MongoDB for GIANT Ideas - Build innovative modern applications that create a competitive advantage.
- [CouchDB](http://couchdb.apache.org/) - Apache CouchDB is open source database software that focuses on ease of use and having an architecture that "completely embraces the Web".
- [Couchbase](http://www.couchbase.com/) - NoSQL database is developed by Couchbase.
- [DocumentDB](https://azure.microsoft.com/en-us/services/documentdb/) - DocumentDB is a fully managed NoSQL database service built for fast and predictable performance, high availability, elastic scaling.
- [IBM Cloudant](https://cloudant.com/) - IBM® Cloudant® is a managed NoSQL JSON database service built to ensure that the flow of data between an application and its database.

### Search DB
- [Elasticsearch](https://www.elastic.co/products/elasticsearch) - Elasticsearch is a distributed, RESTful search and analytics engine capable of solving a growing number of use cases.
- [Apache Solr](https://lucene.apache.org/solr/) - Solr is highly reliable, scalable and fault tolerant, providing distributed indexing, replication and load-balanced querying.
- [Splunk](https://www.splunk.com/) - Splunk Inc. provides the leading platform for Operational Intelligence. Customers use Splunk to search, monitor, analyze and visualize machine data.

### Graph DB
- [Neo4j](https://neo4j.com/) - Neo4j is a graph database management system developed by Neo Technology, Inc.
- [DataStax Enterprise Graph](https://www.datastax.com/products/datastax-enterprise-graph) - DataStax Enterprise Graph is the first graph database fast enough to power customer facing applications, capable of scaling to massive datasets and advanced integrated tools capable of powering deep analytical queries.
- [Titan](http://titan.thinkaurelius.com/) - Titan is a scalable graph database optimized for storing and querying graphs containing hundreds of billions of vertices and edges distributed across clusters.
- [GraphX](http://spark.apache.org/graphx/) - GraphX is Apache Spark's API for graphs and graph-parallel computation, with a built-in library of common algorithms.

### NewSQL
- [NouDB](http://www.nuodb.com/) - NuoDB is a database startup company based in Cambridge, Massachusetts. It sells a NewSQL database that works in the cloud.
- [FoundationDB](http://www.foundationdb.com/) - FoundationDB was a multi-model NoSQL database with a shared nothing architecture.

### In-memory DB
- [Oracle Database In-Memory](https://www.oracle.com/database/database-in-memory/index.html) - Oracle Database In-Memory delivers leading-edge in-memory performance without the need to restrict functionality or accept compromises, complexity and risk.
- [DB2 BLU](http://www.ibmbluhub.com/) - BLU Acceleration is revolutionary in-memory technology that is designed for high-performance analytics and data-intensive reporting.
- [IBM dashDB](https://console.ng.bluemix.net/catalog/services/dashdb) - IBM dashDB offers fully-managed, SQL database services.
- [Hekaton](https://www.microsoft.com/en-us/research/publication/hekaton-sql-servers-memory-optimized-oltp-engine/) - Hekaton is a new database engine optimized for memory resident data and OLTP workloads.
- [Apache Kudu](http://kudu.apache.org/) - Apache Kudu completes Hadoop's storage layer to enable fast analytics on fast data.
- [Redis](http://redis.io/) - Redis is an open source (BSD licensed), in-memory data structure store, used as database, cache and message broker.
- [VoltDB](https://www.voltdb.com/) - VoltDB is the world's fastest in-memory operational database - allowing you to ingest data, analyze data, and act on data in milliseconds with real-time experience.
- [MemcacheDB](http://memcachedb.org/) - MemcacheDB is a distributed key-value storage system designed for persistent.
- [Pivotal GemFire](https://pivotal.io/big-data/pivotal-gemfire) - Pivotal GemFire is an in-memory distributed data grid for high scale custom applications.
- [Apache Geode](http://geode.apache.org/) - Apache Geode is a distributed, in-memory database with strong data consistency.
- [H2](http://www.h2database.com/) - H2 is a relational database management system written in Java. It can be embedded in Java applications or run in the client-server mode.
- [Hazelcast](https://hazelcast.com/) - Hazelcast is the leading in-memory data grid solution.
- [Ehcache](http://www.ehcache.org/) - Ehcache is an open source, standards-based cache that boosts performance, offloads your database, and simplifies scalability.
- [Infinispan](http://infinispan.org/) - Infinispan is a distributed cache and key-value NoSQL data store software developed by Red Hat.
- [GridGain](https://www.gridgain.com/) - The GridGain Enterprise Edition includes valuable features added to Apache® Ignite™ which make deploying and maintaining a high performance in-memory.
- [Coherence](http://www.oracle.com/technetwork/middleware/coherence/overview/index.html) - Oracle Coherence is the industry leading in-memory data grid solution that enables organizations to predictably scale mission-critical applications by providing fast access to frequently used data.
- [Apache Ignite](https://ignite.apache.org/) - Apache Ignitetm In-Memory Data Fabric is a high-performance, integrated and distributed in-memory platform for computing and transacting.
- [JCS](https://commons.apache.org/proper/commons-jcs/) - JCS is a distributed caching system written in Java.

### Event Store
- [Event Store](https://geteventstore.com/) - The open-source, functional database with Complex Event Processing in JavaScript.

### Embedded Database
- [RocksDB](http://rocksdb.org/) - RocksDB is an embeddable persistent key-value store for fast storage.
- [LevelDB](http://leveldb.org/) - LevelDB is a simple key/value data store built by Google, inspired by BigTable.
- [SQLite](https://sqlite.org/) - SQLite is a relational database management system contained in a C programming library.
- [Berkeley DB](http://www.oracle.com/technetwork/database/database-technologies/berkeleydb/overview/index.html) - Berkeley DB is a family of embedded key-value database libraries providing scalable high-performance data management services to applications.
- [JavaDB](http://www.oracle.com/technetwork/java/javadb/overview/index.html) - Java DB is Oracle's supported distribution of the Apache Derby open source database.
- [Apache Derby](https://db.apache.org/derby/) - Apache Derby, an Apache DB subproject, is an open source relational database implemented entirely in Java and available under the Apache License.

### Time Series
- [Riak TS](http://basho.com/products/riak-ts/) - Riak® TS is the only enterprise-grade NoSQL time series database optimized specifically for IoT and Time Series data.
- [InfluxDB](https://www.influxdata.com/) - InfluxDB is an open-source time series database developed by InfluxData as part of their time series platform. It is written in Go and optimized for fast. 

***********

## Data Warehouse
- [Redshift](https://aws.amazon.com/documentation/redshift/) - Amazon Redshift is a fast, fully managed, petabyte-scale data warehouse service.
- [Vertica](http://www8.hp.com/us/en/software-solutions/advanced-sql-big-data-analytics/) - HPE Vertica 8 introduces a unified architecture and advanced in-database analytics capabilities that enable users to conduct sophisticated analysis at industry-leading scale and speed.
- [Teradata](http://www.teradata.com/) - Teradata is a leading provider of powerful, enterprise big data analytics and services that include Data Warehousing, Data Driven Marketing.
- [Pivotal Greenplum](https://pivotal.io/big-data/pivotal-greenplum) - Pivotal Greenplum is a commercial fully featured data warehouse powered by the open source Greenplum Database.
- [InfiniDB](http://infinidb.co/) - Column Database Accelerates Insights for Analytics, BI, and Data Warehouse.
- [Druid](http://druid.io/) - Druid supports fast aggregations and sub-second OLAP queries.

***********

## Storage
- [Amazon Simple Storage Service (S3)](https://aws.amazon.com/s3/) - Amazon Simple Storage Service (Amazon S3), provides developers and IT teams with secure, durable, highly-scalable cloud storage.
- [Riak S2](http://basho.com/products/riak-s2/) - Riak® S2 is a highly available, scalable, easy-to-operate object storage software solution that’s optimized for holding videos, images, and other files.
- [Ceph Storage](http://ceph.com/ceph-storage/) - Ceph is a distributed object store and file system designed to provide excellent storage.
- [Nimbus.io](https://github.com/SpiderOak/nimbus.io) - Nimbus.io is both a commercially available cloud storage service AND a free software project.
- [OpenStack Swift](http://docs.openstack.org/developer/swift/) - Swift is a highly available, distributed, eventually consistent object/blob store.

***********

## Blockchain
- [Hyperledger](https://www.hyperledger.org/) - Hyperledger is an open source collaborative effort created to advance cross-industry blockchain technologies.

***********

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

![Alt text](resources/Kafka_partition.png?raw=true)

  **Producer is writing to partition 0 of the topic and partition 0 replicates that write to the available replicas.
    A partition can have multiple replicas, each stored on a different broker. 
    One of the replicas is designated as the leader and the rest of the replicas are followers. 
    Internally, Kafka manages all those replicas automatically and makes sure that they are kept in sync. 
    Both the producer and the consumer requests to a partition are served on the leader replica. 
    When a broker fails, partitions with a leader on that broker become temporarily unavailable. 
    Kafka will automatically move the leader of those unavailable partitions to some other replicas to continue serving the client requests. 
    This process is done by one of the Kafka brokers designated as the controller. 
    It involves reading and writing some metadata for each affected partition in ZooKeeper. 
    Currently, operations to ZooKeeper are done serially in the controller. 
    [More Information](https://www.confluent.io/blog/how-to-choose-the-number-of-topicspartitions-in-a-kafka-cluster/)**
    
- [Apache Flume](https://flume.apache.org/) - Flume is a distributed, reliable, and available service for efficiently collecting, aggregating, and moving large amounts of log data.
- [RabbitMQ](https://www.rabbitmq.com/) - RabbitMQ is open source message broker software that implements the Advanced Message Queuing Protocol (AMQP).
- [Mosquitto](https://mosquitto.org/) - Mosquitto is an open source message broker that implements the MQTT (MQ Telemetry Transport) protocol v3.1.
- [Logstash](https://www.elastic.co/products/logstash) - Logstash is an open source, server-side data processing pipeline that ingests data from a multitude of sources simultaneously.
- [Spring XD](http://projects.spring.io/spring-xd/) - Spring XD is a unified, distributed, and extensible service for data ingestion, real time analytics, batch processing, and data export.

### Big Data Speed Layer
- [Kafka Streams](https://www.confluent.io/product/kafka-streams/) - If you use Kafka for stream data transport, the Streams API in Kafka can immediately add stream processing capabilities to your application without the burden of adding an entirely separate distributed processing cluster for another stream processing framework.
- [Akka Streams](http://doc.akka.io/docs/akka/current/scala/stream/index.html) - Asynchronous event processing, integrate with various data sources/sinks, send/receive data over the network or to combine multiple streams.
- [Apache Storm](http://storm.apache.org/) - Apache Storm is a free and open source distributed realtime computation system.
- [Apache Spark Streaming](http://spark.apache.org/streaming/) - Spark Streaming brings Apache Spark's language-integrated API to stream processing, letting you write streaming jobs the same way you write batch jobs.
- [Apache Flume Interceptor](https://flume.apache.org/) - Flume is a distributed, reliable, and available service for efficiently collecting, aggregating, and moving large amounts of log data.
- [Apache Samza](http://samza.apache.org/) - Apache Samza is a distributed stream processing framework. It uses Apache Kafka for messaging, and Apache Hadoop YARN to provide fault tolerance.
- [Apache Gearpump](https://gearpump.apache.org/) - Apache Gearpump is a real-time big data streaming engine.
- [Spring XD](http://projects.spring.io/spring-xd/) - Spring XD is a unified, distributed, and extensible service for data ingestion, real time analytics, batch processing, and data export.
- [Apache Beam](https://beam.apache.org/) - Apache Beam is an open source, unified model and set of language-specific SDKs for defining and executing data processing workflows.

### Big Data Batch Layer
- [Databricks](https://databricks.com/) - Founded by the creators of Apache Spark, Databricks makes big data analytics simple through an integrated workspace hosted as a service in the cloud.
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

***********

## Distributed File System
- [DSEFS](https://docs.datastax.com/en/latest-dse/datastax_enterprise/ana/aboutDsefs.html) - DSEFS (DataStax Enterprise file system) is a new distributed file system within DataStax Enterprise.
- [HDFS](http://hortonworks.com/apache/hdfs/) - HDFS is a Java-based file system that provides scalable and reliable data storage, and it was designed to span large clusters of commodity servers.
- [GlusterFS](https://www.gluster.org/) - GlusterFS is a scalable network filesystem. Using common off-the-shelf hardware, you can create large, distributed storage solutions for media streaming.
- [Amazon EFS](https://aws.amazon.com/efs/) - Shared file storage for the AWS cloud, supporting a file system interface and file system semantics for thousands of Amazon EC2 instances. 
- [Ceph FS](http://docs.ceph.com/docs/jewel/cephfs/) - The Ceph Filesystem (Ceph FS) is a POSIX-compliant filesystem that uses a Ceph Storage Cluster to store its data.
- [Alluxio](http://www.alluxio.org/) - Alluxio, formerly Tachyon, enables any application to interact with any data from any storage system at memory speed.

***********

## BI Tools
- [Tableau](https://www.tableau.com/) - Tableau is data visualization software.
- [Pentaho](http://www.pentaho.com/) - Pentaho's big data integration and analytics solutions turn information into insights to help your organization gain a competitive advantage.
- [Qlik](https://www.qlik.com/) - Qlik delivers Business Intelligence software for data visualization, guided analytics, embedded analytics and reporting to over 40000 customers worldwide.
- [Birt](http://www.eclipse.org/birt/about/) - BIRT is an open source software project that provides the BIRT technology platform to create data visualizations and reports.
- [JasperReports®](http://community.jaspersoft.com/) - The JasperReports Library is the world's most popular open source reporting engine.
- [SAS Visual Analytics](http://www.sas.com/en_us/software/business-intelligence/visual-analytics.html) - Robust reporting and mobile BI.
- [IBM Watson Analytics](https://watson.analytics.ibmcloud.com/product) - Watson Analytics guides analysis with automated data visualization and discovery so you can uncover insights on your own.

***********

## DevOps
- [Docker](https://www.docker.com/) - Docker is an open platform for developers and sysadmins to build, ship, and run distributed applications, whether on laptops, data center VMs, or the cloud.
- [Ansible](https://www.ansible.com/) - Ansible is the simplest way to automate apps and IT infrastructure.
- [Jenkins](https://jenkins.io/) - Jenkins is an open source automation server written in Java.
- [Bamboo](https://www.atlassian.com/software/bamboo) - Continuous delivery, from code to deployment. ... Focus on coding and count on Bamboo as your CI and build server.
- [Chef](https://www.chef.io/chef/) - Chef is an open source software agent that automates your infrastructure by turning it into code.
- [Puppet](https://puppet.com/) - Puppet is an open-source configuration management tool.

***********

## Security
- [OWASP](https://www.owasp.org/) - The Open Web Application Security Project (OWASP) is an online community which creates freely-available articles, methodologies, documentation, tools.
- [OAuth](https://oauth.net/) - OAuth is an open standard for authorization, commonly used as a way for Internet users to authorize websites or applications to access their information on other.
- [SAML](https://en.wikipedia.org/wiki/Security_Assertion_Markup_Language) - Security Assertion Markup Language (SAML, pronounced sam-el) is an XML-based, open-standard data format for exchanging authentication and authorization data.
- [MIT KDC](https://web.mit.edu/kerberos/krb5-devel/doc/admin/install_kdc.html) - Kerberos is a network authentication protocol. It is designed to provide strong authentication for client/server applications by using secret-key cryptography.
- [OpenLDAP](http://www.openldap.org/) - OpenLDAP Software is an open source implementation of the Lightweight Directory Access Protocol.
- [Active Directory](https://en.wikipedia.org/wiki/Active_Directory) - Active Directory (AD) is a directory service that Microsoft developed for Windows domain networks.

***********

## Web Frameworks
- [ReactJS](https://facebook.github.io/react/) - Declarative. React makes it painless to create interactive UIs. Design simple views for each state in your application.
- [AngularJS](https://angularjs.org/) - AngularJS is what HTML would have been, had it been designed for building web-apps. Declarative templates with data-binding, MVW, MVVM, MVC.

***********

## Mobile Frameworks
- [Xamarin](https://www.xamarin.com/) - Xamarin's mobile application development platform with native user interfaces enables sharing of code across all platforms with a single C# codebase.
- [React Native](https://facebook.github.io/react-native/) - Build Native Mobile Apps using JavaScript and React. React Native lets you build mobile apps using only JavaScript. It uses the same design as React. 
- [Apache Cordova](https://cordova.apache.org/) - Apache Cordova (formerly PhoneGap) is a popular mobile application development framework originally created by Nitobi.

***********

## Game Engines
- [Unity3D](https://unity3d.com/) - Unity3D is a cross-platform game engine developed by Unity Technologies and used to develop video games for PC, consoles, mobile devices and websites.
- [Unreal Engine](https://www.unrealengine.com) - Unreal Engine 4 is a suite of integrated tools for game developers to design and build games, simulations, and visualizations.
- [Stingray](http://www.autodesk.com/products/stingray/overview) - Autodesk® Stingray is a modern game engine built on a powerful, data-driven core architecture that can produce visually stunning games.
- [Lumberyard](https://aws.amazon.com/lumberyard/) - Amazon Lumberyard is a free, cross-platform, 3D game engine for you to create the highest-quality games, connect your games to the vast compute and storage. 

***********

## IoT

### IoT OS
- [Brillo](https://developers.google.com/brillo/) - Brillo brings the simplicity and speed of software development to hardware for IoT with an embedded OS, core services, developer kit, and developer console.
- [mbed OS](https://www.mbed.com/en/platform/mbed-os/) - ARM mbed OS is a platform operating system designed for the internet of things.

***********

## UML Tools
- [Draw.io](https://www.draw.io/) - Draw.io is free online diagram software for making flowcharts, process diagrams, org charts, UML, ER and network diagrams.
- [Microsoft Visio](https://products.office.com/en/visio/flowchart-software) - Microsoft Visio (formerly Microsoft Office Visio) is a diagramming and vector graphics application and is part of the Microsoft Office family.
- [Enterprise Architect](http://www.sparxsystems.com/) - Enterprise architects are practitioners of enterprise architecture; an enterprise strategic management discipline that operates within organizations.

***********

## Summit Events
- [AWS re:Invent](https://reinvent.awsevents.com/) - At AWS re:Invent, connect with peers and cloud experts, collaborate at our bootcamps, and learn how AWS can improve productivity, security.
- [Web Summit](https://websummit.net/) - It's been called 'the best technology conference on the planet'.
- [AWS Summit](https://aws.amazon.com/summits/) - Whether you are new to the cloud or an experienced user, you will learn something new at an AWS Summit.
- [Gamescom](http://www.gamescom-cologne.com/) - Gamescom (stylized as gamescom) is a trade fair for video games held annually at the Koelnmesse in Cologne, North Rhine-Westphalia, Germany.
- [GDC](http://www.gdconf.com/) - An event designed to inform and educate game industry professionals on online multiplayer games, mobile and next generation game technologies.
- [Strata Hadoop World](http://www.stratahadoopworld.com/) - Strata Hadoop World. Where big data, cutting-edge data science, and new business fundamentals intersect–and merge.
- [Spark Summit](https://spark-summit.org/) - Organized by Databricks, Spark Summit is the premier big data conference series dedicated to bring the Apache Spark community together across the globe.
- [Reactive Summit](https://www.reactivesummit.org/) - Organized by Lightbend.
- [PyData Events](http://pydata.org/events.html) - PyData is a three-day event where data science professionals, in both academia and enterprise, come together to discuss the challenges.

**[⬆ back to top](#table-of-contents)**

