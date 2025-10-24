## Title

Maximum Gcd

## Slug

maximum-gcd

## Difficulty

Medium

## Description

There are N integers — A₁, A₂, A₃, …, Aₙ — written on a blackboard.
You are allowed to choose one of them and replace it with any integer of your choice between 1 and 10⁹ (inclusive). The new integer may be the same as the original one.

Your task is to find the maximum possible greatest common divisor (GCD) of all N integers on the blackboard after making your move.

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If we replace 7 with 4, the greatest common divisor of the three integers on the blackboard will be 2, which is the maximum possible value.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

We can replace an integer with itself.

## Input Format

- First line: integer 'n' representing the number of elements written on the blackboard .  
- Second line: 'n' integers representing the elements that are written on blackboard.
- You will be given the array as an input to your function

## Output Format

- Return an integer representing the greatest common divisor after making your move.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, suffix sum, math
