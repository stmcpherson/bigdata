Create package:
mvn archetype:generate -DgroupId=org.apache.spark.examples -DartifactId=sparkPi -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

Run:
/home/hadoop/spark/bin/spark-submit --deploy-mode cluster --master yarn-cluster --class org.apache.spark.examples.SparkPi ~/sparkPi/target/sparkPi-1.0-SNAPSHOT.jar 10
