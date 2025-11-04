## Title

The Unmatched Dance Partner

## Slug

unmatched-dance-partner

## Difficulty

Medium

## Description

At a royal ball, dancers are lined up, sorted by their height. Every dancer has a partner of the exact same height, and they stand next to each other. However, one dancer is unique and has no partner. Their height appears only once in the line. Given the sorted list of heights, find the height of the lone dancer.

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

- The first line contains an odd integer n, the total number of dancers.
- The second line contains n space-separated integers representing the sorted heights.

## Output Format

- Return a single integer: the height of the dancer that appears only once.

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