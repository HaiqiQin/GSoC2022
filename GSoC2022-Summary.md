# logging-elasticsearch-plugin-summary



## Problem description

Apache Shenyu is an asynchronous, high-performance, cross language, responsive API gateway.It 
can support multiple languages, has built-in rich plugins, has flexible traffic filtering, and supports 
observability, so as to make the micro service run stably.The observable part is mainly composed 
of metrics，tracing and logging.In the field of logging, Apache Shenyu uses the form of plugins to 
obtain log records related to requests and responses.When calling the target service, Apache 
Shenyu gateway allows users to use the logging plugin to print request information in the log, 
including request path, request method, request parameters, response header, response body 
and other information.Apache Shenyu supports the use of elasticsearch, Kafka and rocketmq to 
obtain gateway log information, but at present, it can only support the use of rocketmq to obtain 
gateway log information.Therefore, the problem to be solved this time is to add the logging 
elasticsearch plugin module to support the acquisition of Apache Shenyu gateway log 
information, and then write it into elasticsearch and display it.



## Main PR link

 **loggingElasticSearch plugin**

- https://github.com/apache/shenyu/pull/3580
- https://github.com/apache/shenyu/pull/3634

**unit test** 

- https://github.com/apache/shenyu/pull/3591
- https://github.com/apache/shenyu/pull/3642
- https://github.com/apache/shenyu/pull/3626

**integrated test** 

-  https://github.com/apache/shenyu/pull/3624

**doc**

- https://github.com/apache/shenyu-website/pull/623



## Repair of some problems

**add dependency license**

- https://github.com/apache/shenyu/pull/3594

**fix thread pool**

- https://github.com/apache/shenyu/pull/3909

