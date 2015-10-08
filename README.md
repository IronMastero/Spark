# Spark
Spark Installations
#This is Spark installation Alone
#Download spark from Spark website

cd Downloads
tar xvf spark-1.4.0.tgz
cd spark-1.4.0
sbt/sbt  assembly # This will take some time to build.

After installation and build is ready
#test
./bin/run-example SparkPi 10

#Spark Interactive Shell
./bin/spark-shell

scala> val textFile = sc.textFile("README.md")
textFile.count()

#Installing Spark on Hadoop Single Node Cluster 
http://www.bogotobogo.com/Hadoop/BigData_hadoop_Install_on_ubuntu_single_node_cluster.php

#Get Scala 2.10.4 for Spark 1.5.1 
wget http://www.scala-lang.org/files/archive/scala-2.10.4.tgz
tar -xvf scala-2.10.4.tgz
cd scala-2.10.4
export PATH=`pwd`/bin:$PATH
export SCALA_HOME=`pwd`
