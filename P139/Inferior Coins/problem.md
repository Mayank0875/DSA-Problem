## Title
Inferior Coins

## Slug
inferior-coins

## Difficulty
Medium

## Description
A crypto trader evaluates coins.

You have a list of $n$ coins. Each coin has two main properties: **transaction speed** and **security score**. You are given a 2D integer array `properties` where `properties[i] = [transaction speed_i, security score_i]` represents the attributes of the $i$-th coin.

A coin is considered **inferior** if there exists another coin that has **both** strictly greater transaction speed and strictly greater security score.

More formally, the $i$-th coin is inferior if there exists an index $j$ such that `transaction speed_j > transaction speed_i` and `security score_j > security score_i`.

Your task is to return the number of inferior coins.

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
No coin has strictly greater transaction speed and security score than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first coin (2, 2) is inferior because the second coin (3, 3) has strictly greater transaction speed and security score.

## Input Format
- The first line contains an integer $n$, the number of coins.
- The next $n$ lines each contain two space-separated integers, representing the transaction speed and security score of a coin.

## Output Format
- Return a single integer representing the number of inferior coins.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ transaction speed, security score ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
