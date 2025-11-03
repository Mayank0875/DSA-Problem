## Title

Cycled Duty Roster

## Slug

cycled-duty-roster

## Difficulty

Medium

## Description

A military duty roster lists soldier IDs, originally sorted in ascending order. The daily roster is "cycled" or "rotated" from this master list, starting at a different soldier each day (e.g., [1, 2, 3, 4] becomes [3, 4, 1, 2]). You are given today's cycled list of unique IDs and a specific soldier's ID to find. You must find the soldier's index in O(log n) time, or return -1 if they are not on the list.

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