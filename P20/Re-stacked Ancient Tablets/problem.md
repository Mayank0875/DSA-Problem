## Title

Re-stacked Ancient Tablets

## Slug

re-stacked-ancient-tablets

## Difficulty

Medium

## Description

An archaeologist found a stack of ancient tablets, numbered sequentially. They discovered the stack was "cut" at some point, and the bottom part was moved to the top, creating a rotated sorted array of tablet IDs (e.g., [1, 2, 3, 4, 5] became [4, 5, 1, 2, 3]). Given this array of unique IDs and a target ID, find the tablet's index in O(log n) time. If the tablet is not in the stack, return -1.

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