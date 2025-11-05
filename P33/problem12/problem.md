## Title

Story Arc Climax

## Slug

story-arc-climax

## Difficulty

Medium

## Description

You are analyzing the dramatic tension of a story, represented by `n` data points. The tension builds to a climax (a peak) and then resolves (decreases). This forms a "mountain array":
    1. n >= 3
    2. `tension[0] < tension[1] < ... < tension[i-1] < tension[i]`
    3. `tension[i] > tension[i+1] > ... > tension[n-1]`

Find the index of the story's climax (the point of maximum tension).

## Examples

### 1

#### Input

7
[0, 1, 2, 4, 2, 1, 0]

#### Output

3

#### Explanation

The array is [0, 1, 2, 4, 2, 1, 0]. The peak element is 4 at index 3.

### 2

#### Input

5
[1, 5, 4, 3, 2]

#### Output

1

#### Explanation

The array is [1, 5, 4, 3, 2]. The peak element is 5 at index 1.

## Input Format

- The first line contains a single integer n, the number of elements in the array.
- The second line contains n space-separated integers, representing the elements of the mountain array arr.

## Output Format

- Return a single integer: the index of the peak element.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9
- The input array is guaranteed to be a mountain array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory