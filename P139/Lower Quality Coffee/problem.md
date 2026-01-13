## Title
Lower Quality Coffee

## Slug
lower-quality-coffee

## Difficulty
Medium

## Description
A barista grades coffee beans.

You have a list of $n$ beans. Each bean batch has two main properties: **aroma score** and **flavor score**. You are given a 2D integer array `properties` where `properties[i] = [aroma score_i, flavor score_i]` represents the attributes of the $i$-th bean batch.

A bean batch is considered **lower quality** if there exists another bean batch that has **both** strictly greater aroma score and strictly greater flavor score.

More formally, the $i$-th bean batch is lower quality if there exists an index $j$ such that `aroma score_j > aroma score_i` and `flavor score_j > flavor score_i`.

Your task is to return the number of lower quality beans.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No bean batch has strictly greater aroma score and flavor score than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first bean batch (2, 2) is lower quality because the second bean batch (3, 3) has strictly greater aroma score and flavor score.

## Input Format
- The first line contains an integer $n$, the number of beans.
- The next $n$ lines each contain two space-separated integers, representing the aroma score and flavor score of a bean batch.

## Output Format
- Return a single integer representing the number of lower quality beans.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ aroma score, flavor score ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
