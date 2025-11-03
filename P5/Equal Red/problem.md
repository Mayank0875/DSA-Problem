## Title

Equal Red/Green Light Cycle

## Slug

equal-red-green-light-cycle

## Difficulty

Easy

## Description

The state of a traffic light over N intervals is recorded, where '0' means the light was red and '1' means it was green. We are looking for the longest continuous sequence of intervals where the total duration (number of intervals) the light was red is equal to the total duration it was green. This represents the longest balanced cycle. Find the length of the longest such sequence.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The sequence [0, 1] (Red, Green) is the longest balanced cycle.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] (Red, Green) and [1, 0] (Green, Red) are the longest balanced cycles.

## Input Format

- The first line contains a single integer N, the number of intervals recorded.
- The second line contains N space-separated integers, representing the light state (0 for red, 1 for green).

## Output Format

- Return a single integer representing the length of the longest contiguous sequence with an equal number of 0s and 1s.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hashmap