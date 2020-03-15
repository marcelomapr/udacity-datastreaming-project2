# udacity-datastreaming-project2
Project 2 for the Data Streaming course at Udacity

## How did changing values on the SparkSession property parameters affect the throughput and latency of the data?
It impacts the processedRowsPerSecond.

## What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal?
The most efficient for me were spark.sql.shuffle.partitions (set to 10) and the spark.default.parallelism (set to 11000). I monitored the processedRowsPerSecond measure in order to figure out which specifications were the most optimal.