## Title

Traffic Light Synchronization

## Slug

traffic-light-synchronization

## Difficulty

Medium

## Description

A street has N traffic lights in a row. Each light is either 'Red' (0) or 'Green' (1). For traffic to flow smoothly, the entire street must have an equal number of red and green lights. A traffic engineer can "decommission" exactly one contiguous segment of lights to achieve this balance. What is the shortest segment of lights they must remove? If the street is already balanced, the length is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The street has four 'Red' (0) and two 'Green' (1) lights. To balance, we must remove two more 0s than 1s.
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