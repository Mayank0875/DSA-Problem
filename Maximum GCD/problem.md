## Title

Maximum Gcd

## Slug

maximum-gcd

## Difficulty

Medium

## Description

There are N integers A1, A2, A3 ... An, written on the blackboard.
You will be choosen one of them and replace it with any integer of your choice bewteen 1 to 1e9 (inclusive) possible the same integer originally written.

Find the Maximum possible greatest common divisior of the N integers on the blackboard after your move.

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

- Return an integer representing the greatest common divisor.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, suffix sum, math
