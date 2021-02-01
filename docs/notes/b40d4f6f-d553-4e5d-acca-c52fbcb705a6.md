---
id: b40d4f6f-d553-4e5d-acca-c52fbcb705a6
title: Spark
desc: ''
updated: 1612181799057
created: 1612181799057
parent: 6a4a312f-8ff9-400c-888c-d33848bd2d14
children:
  - 55cf1b3f-70e4-4676-afb5-ef6c3e879a0e
  - ff732bcd-2ee6-4ef5-9e52-557073dd7e8c
fname: spark
hpath: spark
---
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

