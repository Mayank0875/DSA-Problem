## Title
Less Qualified Candidates

## Slug
less-qualified-candidates

## Difficulty
Medium

## Description
HR screens job applicants.

You have a list of $n$ candidates. Each candidate has two main properties: **years of experience** and **skill score**. You are given a 2D integer array `properties` where `properties[i] = [years of experience_i, skill score_i]` represents the attributes of the $i$-th candidate.

A candidate is considered **less qualified** if there exists another candidate that has **both** strictly greater years of experience and strictly greater skill score.

More formally, the $i$-th candidate is less qualified if there exists an index $j$ such that `years of experience_j > years of experience_i` and `skill score_j > skill score_i`.

Your task is to return the number of less qualified candidates.

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
No candidate has strictly greater years of experience and skill score than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first candidate (2, 2) is less qualified because the second candidate (3, 3) has strictly greater years of experience and skill score.

## Input Format
- The first line contains an integer $n$, the number of candidates.
- The next $n$ lines each contain two space-separated integers, representing the years of experience and skill score of a candidate.

## Output Format
- Return a single integer representing the number of less qualified candidates.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ years of experience, skill score ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
