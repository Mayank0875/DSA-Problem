## Title

Unbalanced Element

## Slug

unbalanced-element

## Difficulty

Medium

## Description

In a magical ceremony, `n` power stones are placed in a line, sorted by their energy frequency. To maintain balance, every stone must be paired with another of the exact same frequency. In your line of stones, one stone is "unbalanced" and appears only once. Find the frequency of this unbalanced stone.

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

- The first line contains an odd integer n, the total number of stones.
- The second line contains n space-separated integers representing the sorted energy frequencies.

## Output Format

- Return a single integer: the frequency of the stone that appears only once.

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