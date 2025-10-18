## Title

Spun Key Ring Search

## Slug

spun-key-ring-search

## Difficulty

Medium

## Description

Imagine you have a large key ring where keys are numbered and originally arranged in increasing order. 
Someone spun the ring, so the sequence of key numbers is now shifted. 
For example, keys numbered [1, 2, 3, 4, 5, 6] might now appear as [4, 5, 6, 1, 2, 3]. 
All key numbers on the ring are unique. Given this spun sequence of keys and the number of a specific key you're looking for, your task is to find the position (index) of that key on the ring. If the key isn't there, you should report that.

You must write an algorithm with O(log n) runtime complexity

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

binary-search, array, rotated-array
