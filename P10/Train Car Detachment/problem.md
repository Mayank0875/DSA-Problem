## Title

Train Car Detachment

## Slug

train-car-detachment

## Difficulty

Medium

## Description

A train consists of N cars, each designated as either 'Passenger' (1) or 'Cargo' (0). For a "mixed-freight" train to be valid, it must have an equal number of passenger and cargo cars. The train conductor can detach exactly one contiguous segment of cars. What is the length of the shortest segment that can be detached to make the remaining train valid? If the train is already valid, return 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The train has four 'Cargo' (0) and two 'Passenger' (1) cars. To balance, we must remove two more 0s than 1s.
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