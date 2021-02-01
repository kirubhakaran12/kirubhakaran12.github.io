### Spark Basics

<b>SparkContext</b> - tells Spark how to access a cluster
<b>SparkSparkConfContext</b> - contains information about application

```python
from pyspark import SparkContext, SparkConf

conf = SparkConf().setAppName(appName).setMaster(master)
sc = SparkContext(conf=conf)
```

master -  Spark, Mesos or YARN cluster URL

### Launching ushing shell

```sh
$ ./bin/pyspark --master local[4]
$ ./bin/pyspark --master local[4] --py-files code.py
```