## Title
Server Load Spike

## Slug
server-load-spike

## Difficulty
Easy

## Description
An admin monitors n load samples. They want to detect a pattern of strictly increasing load.

You have n load percentage samples.
A load spike pattern consists of samples where the load is strictly higher than the previous sample.

You must detect pattern to find the longest possible load spike. You can skip any number of samples to form the sequence, but you must maintain the original time order of the selected samples. Calculate the maximum number of samples that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest load spikes (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 sample.

## Input Format
- The first line contains an integer n: the number of samples.
- The second line contains n integers x_1, x_2 ... x_n: the load of each sample in order.

## Output Format
- Return one integer: the length of the longest valid load spike.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
