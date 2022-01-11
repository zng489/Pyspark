
# What's RDD...
### http://vishnuviswanath.com/spark_rdd.html

Spark RDDs are very simple at the same time very important concept in Apache Spark. Most of you might be knowing the full form of RDD, it is Resilient Distributed Datasets. Resilient because RDDs are immutable(can’t be modified once created) and fault tolerant, Distributed because it is distributed across cluster and Dataset because it holds data.

So why RDD? Apache Spark lets you treat your input files almost like any other variable, which you cannot do in Hadoop MapReduce. RDDs are automatically distributed across the network by means of Partitions.

Partitions

RDDs are divided into smaller chunks called Partitions, and when you execute some action, a task is launched per partition. So it means, the more the number of partitions, the more the parallelism. Spark automatically decides the number of partitions that an RDD has to be divided into but you can also specify the number of partitions when creating an RDD. These partitions of an RDD is distributed across all the nodes in the network.

---