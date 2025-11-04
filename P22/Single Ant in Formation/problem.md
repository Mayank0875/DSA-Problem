## Title

Single Ant in Formation

## Slug

single-ant-in-formation

## Difficulty

Medium

## Description

An ant colony marches in a sorted line, based on their size. They march in pairs, side-by-side. However, one ant is marching alone. This ant's size appears only once in the sorted list, while all other sizes appear twice. Find the size of this single ant.

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

- The first line contains an odd integer n, the total number of ants.
- The second line contains n space-separated integers representing the sorted ant sizes.

## Output Format

- Return a single integer: the size of the ant that appears only once.

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