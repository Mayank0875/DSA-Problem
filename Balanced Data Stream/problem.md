## Title

Balanced Data Stream

## Slug

balanced-data-stream

## Difficulty

Medium

## Description

An AI archivist, Unit 734, is processing a massive binary data stream. For the data to be stable for long-term storage, the number of 0s and 1s in the stream must be perfectly equal. 
Unit 734 can achieve this balance by removing exactly one contiguous segment from the stream. Your task is to help the archivist by finding the length of the shortest possible contiguous segment that must be removed. 
If the stream is already balanced, no segment needs to be removed, and the length is 0.


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