## Title

Smallest Missing Positive

## Slug

smallest-missing-positive

## Difficulty

Medium

## Description

You are given an unsorted integer array `nums`.

Your task is to find the smallest positive integer that is **not present** in the array.

For example, if the array contains `[1, 2, 0]`, the smallest missing positive integer is `3`. If the array contains `[3, 4, -1, 1]`, the missing integer is `2`.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input

3
1 2 0

#### Output

3

#### Explanation

The integers 1 and 2 are present. The smallest missing positive is 3.
    
### 2

#### Input

4
3 4 -1 1

#### Output

1

#### Explanation

1 is present, but 2 is missing.

## Input Format  

- The first line contains an integer $n$, the size of the array.
- The second line contains $n$ space-separated integers `nums`.

## Output Format  

- Return a single integer representing the smallest missing positive number.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- -1e9 ≤ n ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, two-pointers

## Company
grab