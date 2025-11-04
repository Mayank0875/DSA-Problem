## Title

The Lone Wolf

## Slug

the-lone-wolf

## Difficulty

Medium

## Description

A wolf pack is lined up for inspection, sorted by their "rank" (an integer). Wolves always operate in pairs, so each rank number should appear twice in a row. However, one legendary "Lone Wolf" is in the line-up, and their rank appears only once. Find the rank of the Lone Wolf.

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

- The first line contains an odd integer n, the total number of wolves.
- The second line contains n space-separated integers representing the sorted ranks.

## Output Format

- Return a single integer: the rank of the wolf that appears only once.

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