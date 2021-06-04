# Graph-Embedding Based Clustering for Log Anomaly Detection

## Overview

To detect anomalies in large console log series, we propose a novel clustering method with graph-embedding. We leverage both the semantic knowledge and relationship among individual log messages to create meaningful and robust embedding for each event. The embedding is then aggregated to form sequence feature vectors for log anomaly detection through clustering and distance weighing. With the employment of efficient clustering assignment model, we reduce the offline computation time and complexity while preserving the distinct identification of anomalies.

## Train and Test Models

The main pipeline of our research is documented in `method` section, and you can run the Jupiter notebook to get the similar visualization and experimental result as our uploaded one.

Our entire developing and testing process, including different implementations for sequence embedding methods, is documented in `test` section. It is used mainly for our development purpose, but you can still see how the performance changes as we switch between different methods.

## Experiment Results

Followings are some visualization results for (1) training clustering, (2) testing clustering, and (3) the final metrics we achieve:

![train clustering](https://github.com/MarioMZhang/Anomaly-log-detection/blob/main/assets/seq_embed_trn.png)
![train clustering](https://github.com/MarioMZhang/Anomaly-log-detection/blob/main/assets/seq_embed_tst.png)
![train clustering](https://github.com/MarioMZhang/Anomaly-log-detection/blob/main/assets/pred_eval.png)