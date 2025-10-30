## Title

Survey Data Sanitization

## Slug

survey-data-sanitization

## Difficulty

Medium

## Description

You are given N survey responses, where each response is either 'No' (0) or 'Yes' (1). To ensure the data is not biased, you must have an equal number of 'Yes' and 'No' responses. You can sanitize the data by removing exactly one contiguous block of responses. Your task is to find the length of the shortest block you can remove to equalize the 'Yes' and 'No' counts. If the data is already balanced, the length is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The data has four 'No' (0) and two 'Yes' (1). To balance, we need to remove a segment with two more 0s than 1s.
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