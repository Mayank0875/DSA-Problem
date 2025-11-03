## Title

Rotated Star Chart

## Slug

rotated-star-chart

## Difficulty

Medium

## Description

You are a navigator on a spaceship. The ship's star chart is a list of star systems sorted by their unique ID numbers. However, the chart display is circular and has been rotated, so the list starts from an unknown system (e.g., [1, 2, 3, 4, 5, 6] might become [4, 5, 6, 1, 2, 3]). Given this rotated list of unique IDs, find the index of a target star system. You must write an algorithm with O(log n) runtime complexity.

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