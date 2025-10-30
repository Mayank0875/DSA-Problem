## Title

Stock Market Correction

## Slug

stock-market-correction

## Difficulty

Medium

## Description

You are analyzing N days of stock market data. Each day is recorded as either a 'Loss' (0) or a 'Gain' (1). A "stable period" is defined as having an equal number of gain and loss days. You suspect that one anomalous, contiguous period is skewing the data. Find the length of the shortest contiguous period of days that can be removed from the record to make the remaining data "stable." If the record is already stable, the length is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The record has four 'Loss' (0) days and two 'Gain' (1) days. To balance, we need to remove a period with two more 0s than 1s.
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