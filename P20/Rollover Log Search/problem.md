## Title

Rollover Log Search

## Slug

rollover-log-search

## Difficulty

Medium

## Description

A system log file contains entries sorted by a unique timestamp. When the log reaches its maximum size, it "rolls over," placing new entries at the beginning while the oldest entries are at the end. This creates a rotated sorted array of timestamps (e.g., [50, 60, 10, 20, 30]). You are given this array and a target timestamp. Find the index of the target entry in O(log n) time, or return -1 if it's not present.

## Examples

### 1

#### Input

7 0 
[4, 5, 6, 7, 0, 1, 2]


#### Output

4

#### Explanation

The key numbered 0 is at position 4 on the spun key ring.

### 2

#### Input

7 3 
[4, 5, 6, 7, 0, 1, 2]

#### Output

-1

#### Explanation

The key numbered 3 is not on this key ring.

## Input Format

- The first line contains an integers n and target , the number of keys on the ring and the number of the key to find.
- The second line contains n space-separated integers representing the key numbers after the ring was spun. All numbers are unique.

## Output Format

- Return the index (0-based position) of the target key if it exists else -1 if the target key is not found.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ key_number, target ≤ 10^9
- The array is a rotation of a sorted array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array