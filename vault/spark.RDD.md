
#### Create RDD

```python
data = [1, 2, 3, 4, 5]
distData = sc.parallelize(data)
```

### Loading External Files

```python
distFile = sc.textFile("data.txt")
distFile = sc.textFile("/my/directory")
distFile = sc.textFile("/my/directory/*.txt")
distFile = sc.textFile("/my/directory/*.gz")
```

### Save as sequential files

```python
rdd = sc.parallelize(range(1, 4)).map(lambda x: (x, "a" * x))
rdd.saveAsSequenceFile("path/to/file")
sorted(sc.sequenceFile("path/to/file").collect())
```
### Operations