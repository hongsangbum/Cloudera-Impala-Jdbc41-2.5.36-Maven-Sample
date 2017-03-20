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

4. find possible idencital jar on maven repository

jar file                   | diff yn  | groupid                   | artifactId      | version 
-------------------------- | -------- | ------------------------- | --------------- | ------- 
commons-codec-1.3.jar      | Y        | commons-codec             | commons-codec   | 1.3     
libfb303-0.9.0.jar         | Y        | org.apache.thrift         | libfb303        | 0.9.0   
libthrift-0.9.0.jar        | Y        | org.apache.thrift         | libthrift       | 0.9.0 
log4j-1.2.14.jar           | Y        | log4j                     | log4j           | 1.2.14 
slf4j-api-1.5.11.jar       | Y        | org.slf4j                 | slf4j-api       | 1.5.11 
slf4j-log4j12-1.5.11.jar   | Y        | org.slf4j                 | slf4j-log4j12   | 1.5.11 
zookeeper-3.4.6.jar        | Y        | org.apache.zookeeper      | zookeeper       | 3.4.6 


5. clodera own jars

groupId and artifactId and version is your choice. hive-metastore and hive-service have maven repositories,
but i giveup find mached maven version. 
attached hive-metastore.jar contains below list classes

C:\Users\jason\Downloads\impala_jdbc_2.5.36.2056\2.5.36.1056 GA\Cloudera_ImpalaJDBC41_2.5.36\hive_metastore\org\apache\hadoop\hive\metastore\api
````
2013-11-29  오후 04:50               918 AlreadyExistsException$1.class
2013-11-29  오후 04:50             3,166 AlreadyExistsException$AlreadyExistsExceptionStandardScheme.class
2013-11-29  오후 04:50             1,384 AlreadyExistsException$AlreadyExistsExceptionStandardSchemeFactory.class
2013-11-29  오후 04:50             2,665 AlreadyExistsException$AlreadyExistsExceptionTupleScheme.class
2013-11-29  오후 04:50             1,366 AlreadyExistsException$AlreadyExistsExceptionTupleSchemeFactory.class
......
2013-11-29  오후 04:50            10,327 UnknownTableException.class
2013-11-29  오후 04:50               867 Version$1.class
2013-11-29  오후 04:50             3,146 Version$VersionStandardScheme.class
2013-11-29  오후 04:50             1,159 Version$VersionStandardSchemeFactory.class
2013-11-29  오후 04:50             2,620 Version$VersionTupleScheme.class
2013-11-29  오후 04:50             1,141 Version$VersionTupleSchemeFactory.class
2013-11-29  오후 04:50             3,100 Version$_Fields.class
2013-11-29  오후 04:50            11,231 Version.class
            1437 file           7,249,352 byte
````


jar file                   | groupid                   | artifactId      | version 
-------------------------- | ------------------------- | --------------- | ------- 
hive_metastore.jar         | impala                    | hive-metastore  | 2.5.36     
hive_service.jar           | impala                    | hive-service    | 2.5.36   
ImpalaJDBC41.jar           | impala                    | impala-jdbc     | 2.5.36 
ql.jar                     | impala                    | ql              | 2.5.36 
TCLIServiceClient.jar      | impala                    | tcliservice     | 2.5.36 

Accoding to https://www.cloudera.com/documentation/enterprise/release-notes/topics/cdh_vd_cdh5_maven_repo_510x.html#maven_510x 

groupId                | artifactId         | version 
---------------------- | ------------------ | --------
org.apache.hive        | hive-metastore     | 1.1.0-cdh5.10.0
org.apache.hive        | hive-service	     | 1.1.0-cdh5.10.0
org.apache.zookeeper   | zookeeper          | 3.4.5-cdh5.10.0

zookeeper version is lower than downloaded jdbc connector.


*. reference 
https://www.cloudera.com/documentation/enterprise/latest/topics/impala_jdbc.html#impala_jdbc
https://github.com/onefoursix/Cloudera-Impala-JDBC-Example
https://github.com/cloudera/Impala
