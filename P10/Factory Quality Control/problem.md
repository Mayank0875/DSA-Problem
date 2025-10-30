## Title

Factory Quality Control

## Slug

factory-quality-control

## Difficulty

Medium

## Description

A factory production line creates N items, each inspected and marked as 'Passed' (1) or 'Failed' (0). For a batch to be valid for shipping, it must contain an equal number of Passed and Failed items. A manager can validate a batch by removing exactly one contiguous segment of items from the line. You must determine the length of the shortest segment that can be removed to validate the batch. If the line is already valid, the length is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The initial line has two 'Passed' (1) and four 'Failed' (0). To balance, we need to remove a segment with two more 0s than 1s.
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