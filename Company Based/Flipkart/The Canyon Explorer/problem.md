## Title

The Canyon Explorer

## Slug

the-canyon-explorer

## Difficulty

Medium

## Description

An explorer is navigating a treacherous canyon filled with floating stone platforms arranged in a straight line. You start at the **first platform** (index 0).

Each platform has a specific stability rating, given by an integer array `platforms`. The value at `platforms[i]` represents the **maximum length** you can jump forward from that position. For example, if you are at index `i` and `platforms[i] = 3`, you can jump to any platform at index `i+1`, `i+2`, or `i+3`.

Your goal is to determine if it is possible to reach the **last platform** (the final index of the array) starting from the first.

Return `true` if you can reach the last platform, or `false` otherwise.

## Examples

### 1

#### Input

5 
2 3 1 1 4

#### Output

true

#### Explanation

Jump 1 step from index 0 to 1, then jump 3 steps to the last index.
    
### 2

#### Input

5 
3 2 1 0 4

#### Output

false

#### Explanation

You will always arrive at index 3 no matter what. Its maximum jump length is 0, which makes it impossible to advance further to the last index.
  

## Input Format  

- The first line contains an integer `n`, the number of platforms.
- The second line contains `n` space-separated integers representing the `platforms` array.

## Output Format  

- Return `true` if the last index is reachable, `false` otherwise.
  

## Constraints  

- 1 ≤ n ≤ 1e4
- 1 ≤ platforms[i] ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, dynamic-programming