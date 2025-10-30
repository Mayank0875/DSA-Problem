## Title

Binary Subroutine

## Slug

binary-subroutine

## Difficulty

Medium

## Description

You are debugging a program that has a binary routine N bits long, stored in an array A. A "stable" routine must contain an equal number of 0s and 1s. You can fix the routine by cutting out exactly one contiguous segment of bits. What is the length of the shortest segment you can cut to make the remaining routine stable? If it's already stable, the length is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The routine has four 0s and two 1s. To balance, we need to remove two more 0s than 1s.
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