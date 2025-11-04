## Title

The Unmatched Key

## Slug

the-unmatched-key

## Difficulty

Medium

## Description

A locksmith has a board with `n` keys, sorted by their cut type (an integer). Every key is supposed to be one of a pair (a key and its duplicate). However, one key is an original master key and has no duplicate. It appears only once. Given the sorted list of key types, find the type of the unique master key.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of keys.
- The second line contains n space-separated integers representing the sorted key types.

## Output Format

- Return a single integer: the key type that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array