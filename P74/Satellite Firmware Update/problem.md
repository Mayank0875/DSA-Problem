## Title
Satellite Firmware Update

## Slug
satellite-firmware-update

## Difficulty
Medium

## Description
Satellites in a constellation form a tree. They update firmware by pairing with a neighbor to verify data. Each satellite verifies with one partner.

The structure is a tree with n satellites and n-1 beams.
A update pair is formed between two satellites connected by a beam.
However, each satellite can be part of at most one update pair.

Your task is to calculate the maximum number of update pairs that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of update pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 update pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form update pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of satellites.
- The next n-1 lines each contain two integers u and v, representing a beam between satellite u and satellite v.

## Output Format
- Return a single integer representing the maximum number of update pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
