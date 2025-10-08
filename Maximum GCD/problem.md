## Title

Ordinary Pairs

## Slug

ordinary-pairs

## Difficulty

Medium

## Description

You are given an array of postive integers, and a postive integer X.
Count the number of ordinary pair (i , j) (1 ≤ i < j ≤ N) that satisfy the following condition:
    1. arr[i] + arr[j] must be divisble by X
    2. arr[i] * arr[j] must be divisble by X


## Examples

### 1

#### Input

3 2
[2, 2, 3]

#### Output

1

#### Explanation

The array is [2, 2, 3] and X = 2.  
Ordinary pairs are (1, 2) because 2 + 2 is divisble by 2 and 2 * 2 is also divisble 2.

### 2

#### Input

4 2
[2, 4, 6, 3]

#### Output

3

#### Explanation

The array is [2, 4, 6, 3] and X = 2.  
Ordinary pairs are (1, 2), (1, 3), (2, 3).

## Input Format

- First line: two integer 'n' and 'X' representing the number of elements in the array and value of X respectively.  
- Second line: 'n' integers representing the elements of the array.
- You will be given the array as an input to your function

## Output Format

- Return an integer representing the number of ordinary pairs.

## Constraints

- 1 ≤ n ≤ 10^6
- 1 ≤ X ≤ 10^6
- 1 ≤ arr[i] ≤ 10^6

## Time Limit

1 second

## Memory Limit

256 MB

## Tags

arrays, two pointers, hashmap, math
