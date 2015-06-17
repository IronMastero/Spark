# Spark
Spark Installations
This is spark installations
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
