## Title

Sensor Array Calibration

## Slug

sensor-array-calibration

## Difficulty

Medium

## Description

You have an array of N sensors. Each sensor reports a binary value, 'Off' (0) or 'On' (1). For the array to be "calibrated," the number of Off and On sensors must be equal. You can calibrate the array by deactivating a single contiguous segment of sensors. Find the minimum number of sensors you must deactivate to achieve calibration. If the array is already calibrated, the answer is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The array has four 'Off' (0) and two 'On' (1) sensors. To balance, we must remove two more 0s than 1s.
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