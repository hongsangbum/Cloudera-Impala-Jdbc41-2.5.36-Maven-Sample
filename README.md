# Cloudera-Impala-Jdbc41-2.5.36-Maven-Sample
Clodera Impala Jdbc Maven Sample based impala_jdbc_2.5.36.2056.zip 

Cloudera Impala Jdbc do not support Maven Repository. Today is 2017-03-17.

This Example is very simular https://github.com/onefoursix/Cloudera-Impala-JDBC-Example .
The differene is Configuaration Way For Maven and Less Typing.

1. Download Jdbc.

   https://www.cloudera.com/downloads/connectors/impala/jdbc/2-5-36.html 

2. Files of Directory

```
C:\Users\user\Downloads\impala_jdbc_2.5.36.2056\2.5.36.1056 GA\Cloudera_ImpalaJDBC41_2.5.36>dir /b *.jar
commons-codec-1.3.jar
commons-logging-1.1.1.jar
hive_metastore.jar
hive_service.jar
httpclient-4.1.3.jar
httpcore-4.1.3.jar
ImpalaJDBC41.jar
libfb303-0.9.0.jar
libthrift-0.9.0.jar
log4j-1.2.14.jar
ql.jar
slf4j-api-1.5.11.jar
slf4j-log4j12-1.5.11.jar
TCLIServiceClient.jar
zookeeper-3.4.6.jar
```

3. find out maven packaged jars above  

jar file                  | maven packaged yn  | groupid                   | artifactId      | version
------------------------- | ------------------ | ------------------------- | --------------- | -------------
commons-codec-1.3.jar     | N                  |                           |                 |
commons-logging-1.1.1.jar | Y                  | commons-logging           | commons-logging | 1.1.1
hive_metastore.jar        | N                  |                           |                 |
hive_service.jar          | N                  |                           |                 |
httpclient-4.1.3.jar      | Y                  | org.apache.httpcomponents | httpclient      | 4.1.3 
httpcore-4.1.3.jar        | Y                  | org.apache.httpcomponents | httpcore        | 4.1.3
ImpalaJDBC41.jar          | N                  |                           |                 |
libfb303-0.9.0.jar        | N                  |                           |                 |
libthrift-0.9.0.jar       | N                  |                           |                 |
log4j-1.2.14.jar          | N                  |                           |                 |
ql.jar                    | N                  |                           |                 |
slf4j-api-1.5.11.jar      | Y                  | org.slf4j                 | slf4j-api       | 1.5.11
slf4j-log4j12-1.5.11.jar  | Y                  | org.slf4j                 | slf4j-log4j12   | 1.5.11
TCLIServiceClient.jar     | N                  |                           |                 |
zookeeper-3.4.6.jar       |                    |                           |                 |




