## Title
Inferior Diamonds

## Slug
inferior-diamonds

## Difficulty
Medium

## Description
A jeweler sorts gemstones.

You have a list of $n$ diamonds. Each diamond has two main properties: **carat weight** and **clarity score**. You are given a 2D integer array `properties` where `properties[i] = [carat weight_i, clarity score_i]` represents the attributes of the $i$-th diamond.

A diamond is considered **inferior** if there exists another diamond that has **both** strictly greater carat weight and strictly greater clarity score.

More formally, the $i$-th diamond is inferior if there exists an index $j$ such that `carat weight_j > carat weight_i` and `clarity score_j > clarity score_i`.

Your task is to return the number of inferior diamonds.

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
No diamond has strictly greater carat weight and clarity score than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first diamond (2, 2) is inferior because the second diamond (3, 3) has strictly greater carat weight and clarity score.

## Input Format
- The first line contains an integer $n$, the number of diamonds.
- The next $n$ lines each contain two space-separated integers, representing the carat weight and clarity score of a diamond.

## Output Format
- Return a single integer representing the number of inferior diamonds.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ carat weight, clarity score ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
