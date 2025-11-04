## Title

The Solo Gem

## Slug

the-solo-gem

## Difficulty

Medium

## Description

A dragon's hoard contains a long line of gemstones, sorted by weight. The dragon loves pairs, so every gem has a partner of identical weight placed next to it. However, one gem is unique and has no partner. Given the sorted list of gem weights, find the weight of this single, solo gem.

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

- The first line contains an odd integer n, the total number of gems.
- The second line contains n space-separated integers representing the sorted gem weights.

## Output Format

- Return a single integer: the weight of the gem that appears only once.

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