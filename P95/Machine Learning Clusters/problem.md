## Title
Machine Learning Clusters

## Slug
machine-learning-clusters

## Difficulty
Hard

## Description
A data scientist clusters data points. Each cluster is labeled by its centroid class, which is the mode of the classes within that cluster.

Dr. Turing has a collection of $n$ data points, where each data point is represented by an integer ID.

To classify the dataset, Dr. Turing must partition these data points into several non-empty clusters. Every data point from the original collection must belong to exactly one cluster. From each cluster, a "centroid label" is extracted. The centroid label is defined as the **mode** (most frequent element) of the data points in that cluster. If a cluster has multiple data points tied for the most frequent appearance, any one of them can be chosen as the centroid label.

Dr. Turing collects all the extracted centroid labels to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> centroid label is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> centroid labels 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> centroid labels 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> centroid labels 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of data points.
- The second line contains $n$ space-separated integers representing the data point IDs.

## Output Format
- Return a single integer representing the number of different multisets of centroid labels possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
