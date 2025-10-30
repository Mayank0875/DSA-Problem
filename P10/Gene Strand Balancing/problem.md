## Title

Gene Strand Balancing

## Slug

gene-strand-balancing

## Difficulty

Medium

## Description

A geneticist is analyzing a DNA strand of length N, represented as a sequence of two base types (0 and 1). For the strand to be "stable" for an experiment, it must contain an equal number of 0s and 1s. The scientist can stabilize the strand by excising exactly one contiguous segment of bases. Your task is to find the length of the shortest segment that can be removed to make the remaining strand stable. If the strand is already stable, the length is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The initial stream has four 0s and two 1s. To balance it, we need to remove two more 0s than 1s. 
The shortest segment that achieves this is [0, 0] at indices 2 and 3. 
The length of the removed segment is 2.


### 2

#### Input

6
[1, 1, 0, 0, 1, 0,]

#### Output

0

#### Explanation

The stream contains three 0s and three 1s. It is already balanced, so no segment needs to be removed. 
The length of the removed segment is 0.


## Input Format

- The first line contains a single integer N, the number of elements in the data stream.
- The second line contains N space-separated integers, where each integer is either 0 or 1.

## Output Format

- Return a single integer representing the length of the shortest contiguous segment that needs to be removed to balance the stream.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, prefix sum, hashmap