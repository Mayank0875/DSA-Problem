## Title

Shifted Library Books

## Slug

shifted-library-books

## Difficulty

Medium

## Description

A library shelf holds books sorted by a unique serial number. A careless intern moved a block of books from the end of the shelf to the beginning, maintaining their order. The result is a "rotated" sorted list (e.g., [101, 102, 103, 104] might become [103, 104, 101, 102]). Given this list and a target serial number, find the book's current position (index) on the shelf. If it's not there, return -1. Your method must be O(log n).

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