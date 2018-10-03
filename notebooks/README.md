# jupyterSpark
## Jupyter Notebooks

Spark is a general purpose cluster computing suit.

1) Batch processing : SQL Like query 
2) Stream processing : new Structured stream: Pandas-dataframe like operations
3) ML Library : built-in support for streaming data 

It also has graph data processing library, but no python api for that :(


  - spark with kafka streaming
  - spark only 
  - example database access code to get sample data from devnet 
  
  
 # How to install: use command: pip3 install: 
 - install spark
 
 - install kafka 
 
 - install kafka-python 
 
If you are runnning the kafka notebook: to run kafka:

 - go to the directory where kafka is installed: 
 
 -- modify the config/server.properties file: We have to set advertised.listeners to PLAINTEXT://localhost:9092
 
 -- start zookeeper:: bin/zookeeper-server-start.sh config/zookeeper.properties 
 
 -- start kafka::  bin/kafka-server-start.sh config/server.properties 

To run the jupyter notebook:go to the directory where the files are: run this comand from the command line : jupyter notebook 


# Demo:

-- first run the kafka producer notebook that will ingest messages to a kafka topic, here, alerts to a topic name 'alerts'
-- then rune the notbook spark reads from kafka . It will listen to that topic and produce output.
 
 # To run in docker: 
 -- https://hub.docker.com/r/jupyter/pyspark-notebook/  or https://github.com/jupyter/docker-stacks/tree/master/all-spark-notebook 
 
 -- this will only work for the spark notebook, not with the kafka notebook.
  
  
 # Helpful links:
 -- https://gist.github.com/rmoff/fb033086b285655ffe7f9ff0582dedbf 
 
 -- https://towardsdatascience.com/getting-started-with-apache-kafka-in-python-604b3250aa05
 
 -- https://blog.sicara.com/get-started-pyspark-jupyter-guide-tutorial-ae2fe84f594f


# Next:
 -- http://docs.h2o.ai/h2o/latest-stable/h2o-docs/flow.html 
 -- http://docs.h2o.ai/sparkling-water/2.3/latest-stable/doc/pysparkling.html 
 -- https://github.com/h2oai/h2o-3/tree/master/examples/deeplearning/notebooks 
 
