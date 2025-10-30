## Title

Light and Dark Magic

## Slug

light-and-dark-magic

## Difficulty

Medium

## Description

A wizard is casting a spell composed of N magical pulses, either 'dark' (0) or 'light' (1). The spell is stable only if the number of dark and light pulses are equal. The wizard can remove one continuous sequence of pulses from the spell to stabilize it. What is the minimum length of a sequence that must be removed? If the spell is already stable, the length is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The spell has four 'dark' (0) and two 'light' (1) pulses. We need to remove a segment with two more 0s than 1s.
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