## Title

Mismatched Element

## Slug

mismatched-element

## Difficulty

Medium

## Description

You are given a sorted list of numbers. In this list, every number appears exactly twice and is adjacent to its pair, except for one number which appears only once. Your task is to find this single, unique number. For example, in `[1, 1, 2, 2, 3, 4, 4]`, the number 3 is the mismatched element.

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

- The first line contains an odd integer n, the total number of elements.
- The second line contains n space-separated integers representing the sorted numbers.

## Output Format

- Return a single integer: the element that appears only once.

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