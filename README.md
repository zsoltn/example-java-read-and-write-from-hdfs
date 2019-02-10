Example for read & write into HDFS
==================

Package for the example : mvn package and get the package in target.

Usage in local MRS servers:

 - $ mvn package
 - login to one of the MRS node 
 - $ source /opt/client/bigdata_env
 - $ yarn jar target/example-java-read-and-write-from-hdfs-1.0-SNAPSHOT-jar-with-dependencies.jar

Usage via MRS Gui  :

 - mvn package (in local, to generate jar file)
 - upload the jar (target/example-java-read-and-write-from-hdfs-1.0-SNAPSHOT-jar-with-dependencies.jar) to OBS bucket 
 - login to OTC console / Service List / Mapreduce Service / Clusters / Select Your Cluster
 - Job Managment / Jobs / Create / create new Mapreduce
 - select URL from OBS 
 - Select "OK"
 - Job List view / View Log / See the output of the JOB 
