## Title

Yin-Yang Alignment

## Slug

yin-yang-alignment

## Difficulty

Medium

## Description

A sequence of N energy orbs is laid out, each being either Yin (0) or Yang (1). For the sequence to be in "harmony," it must contain an equal number of Yin and Yang orbs. You can achieve harmony by removing a single, continuous segment of orbs. Your goal is to find the shortest segment that can be removed to align the energies. If the sequence is already in harmony, the length is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The sequence has four 'Yin' (0) and two 'Yang' (1). To balance, we must remove two more 0s than 1s.
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