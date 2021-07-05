# MapReduce_TechJobs

## Teammates
Joshua Tyndale	jtyndale@rams.colostate.edu
Stephen Harayda	
Dziugas Butkus

## Project
CS455 Term project - Using Spark for Scalable Analytics
Using Apache Spark, a mapreduce implementation was used to analyze 6GB of data, and results were put into visual form.

## Files
indeedProg.py		- PySpark code to break down and analyze indeed job data
kaggleProg.py		- PySpark code to break down and analyze housing data from craigslist

##start master and workers
tick:~/spark/latest$ ./sbin/start-all.sh

##submit jobs to master
tick:~/pySpark$ $SPARK_HOME/bin/spark-submit --master spark://tick:30155 indeedProg1.py

## stop masters and workers
tick:~/spark/latest$ ./sbin/stop-all.sh

##config setup
Spark-env.sh
export SPARK_MASTER_IP=tick
export SPARK_MASTER_PORT=30155
export SPARK_MASTER_WEBUI_PORT=30166
export SPARK_WORKER_CORES=2
export SPARK_WORKER_MEMORY=2g
export SPARK_WORKER_INSTANCES=2

Slaves:
maggot
mosquito
lice
preying-mantis
moth
wasp
weevil
deer-fly
dragonfly
dung-beetle


spark-defaults.conf
spark.master                     spark://tick:30155


#Rent By Region


<img src="https://github.com/jtyndale9/MapReduce_TechJobs/blob/main/rentByRegionGraph.png" width=250><br>


#Rent By State


<img src="https://github.com/jtyndale9/MapReduce_TechJobs/blob/main/StatesGraph.png" width=250><br>

#Highest Cost Cities


<img src="https://github.com/jtyndale9/MapReduce_TechJobs/blob/main/Cost_match_cities_graph.png" width=250><br>

#Listings By Region


<img src="https://github.com/jtyndale9/MapReduce_TechJobs/blob/main/RegionsMostListingsGraph.png" width=250><br>

#Companies Hiring the most


<img src="https://github.com/jtyndale9/MapReduce_TechJobs/blob/main/CompaniesGraph.png" width=250><br>
