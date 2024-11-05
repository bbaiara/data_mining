# Clustering Algorithms: DBSCAN and KMeans/KMeans++

Java implementations of **DBSCAN** and **KMeans/KMeans++** for clustering multidimensional data.

## Overview

### DBSCAN
Density-based algorithm to find clusters and detect outliers.
- **Parameters**:
  - `eps`: Neighborhood radius.
  - `minPts`: Minimum points to form a dense cluster.

### KMeans/KMeans++
Partitioning algorithm that clusters data into `k` groups, with KMeans++ for improved initialization.

## Requirements
- Java Development Kit (JDK) 8 or higher.

## Compilation and Execution

1. **Compile** each Java file:
   ```bash
   javac DBScan.java
   javac KMeans.java
   ```

2. **Run** the algorithms with the following commands.

### Running DBSCAN

```bash
java DBScan <input-file> <minPts> <eps>
```
- **Example**: `java DBScan data.csv 4 1.0`

### Running KMeans/KMeans++

```bash
java KMeans <input-file> [k]
```
- **Example**: `java KMeans data.csv 5`

If `k` is omitted, the program estimates it using an elbow method.


