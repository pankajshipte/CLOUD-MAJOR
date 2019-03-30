Data as a Service

- Dependencies:
	- Hadoop Cluster for HDFS (http://www.bogotobogo.com/Hadoop/BigData_hadoop_Install_on_ubuntu_single_node_cluster.php )
	- Spark Cluster for Spark SQL processing (http://spark.apache.org/downloads.html)
	- Web2py for appserver
	

- Installation(Tested on Hadoop 2.6 and Spark 1.5.2:
	- After Hadoop cluster installation, Deploy FileServer.py on namenode and run as:
		python FileServer.py 5554
	- After Spark cluster installation, Deploy SparkServer.py on Spark master and run as:
		python SparkServer.py 5555
	- Deploy  web2py.app.Dataasservice.w2p to Spark master with Web2py running by importing as existing applications
		Run web2py on port 8000
	- The app has been setup.

- App URL: http://localhost:8000/Dataasservice/default/index
- Monitoring:
	- HDFS namenode: http://localhost:50070/
	- Spark Cluster: http://localhost:8080

- Youtbue Link: https://www.youtube.com/watch?v=lJNrMItr4Fs





	
