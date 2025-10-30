## Title

Harmonious Recipe

## Slug

harmonious-recipe

## Difficulty

Medium

## Description

A recipe involves N steps performed in order. Each step `i` adds `A[i]` "flavor points" (an integer from 0 to 9) to the dish.
A "harmonious segment" of the recipe is a contiguous block of steps, from L to R, where the total flavor points added (`A[L] + ... + A[R]`) is exactly equal to the number of steps in the segment (R - L + 1).
Your task is to count how many harmonious segments exist in the recipe.

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 harmonious segments: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 harmonious segments: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of harmonious segments.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map