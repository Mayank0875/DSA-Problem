## Title

The Odd-One-Out Coin

## Slug

odd-one-out-coin

## Difficulty

Medium

## Description

A coin collector has a display of coins, sorted by year. Every coin is part of a pair (e.g., one "heads" up, one "tails" up), so each year should appear twice. However, one special coin is unique and has no pair; its year appears only once. Find the year of this unique coin.

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

- The first line contains an odd integer n, the total number of coins.
- The second line contains n space-separated integers representing the sorted years.

## Output Format

- Return a single integer: the year of the coin that appears only once.

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