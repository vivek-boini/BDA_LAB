# Spark 6 Experiments Execution Commands

## Start Spark Cluster
```bash
$SPARK_HOME/sbin/start-all.sh
```
## check master node running
```bash
jps
```

## Run Experiments

### 1. Fraud Detection
```bash
spark-submit --master spark://$HOSTNAME:7077 fraud_detection.py
```

### 2. Log Batch Analysis
```bash
spark-submit --master spark://$HOSTNAME:7077 log_batch_analysis.py
```

### 3. Movie Recommendation
```bash
spark-submit --master spark://$HOSTNAME:7077 movie_recommendation.py
```

### 4. News Clustering
```bash
spark-submit --master spark://$HOSTNAME:7077 news_clustering.py
```

### 5. Spark NLP Sentiment
```bash
spark-submit --master spark://$HOSTNAME:7077 spark_nlp_sentiment.py
```

### 6. Spark Word Count
```bash
spark-submit --master spark://$HOSTNAME:7077 spark_wordcount.py
```

## Run in Local Mode (Alternative)
```bash
spark-submit --master local[*] filename.py
```

## Stop Spark Cluster
```bash
$SPARK_HOME/sbin/stop-all.sh
```