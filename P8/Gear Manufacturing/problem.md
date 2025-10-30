## Title

Gear Manufacturing

## Slug

gear-manufacturing

## Difficulty

Medium

## Description

A machine contains N gears, `A[1]` to `A[N]`, where `A[i]` is the number of teeth on the i-th gear. For the machine to run smoothly, the number of teeth on all gears should share a large common divisor. A technician can re-mill exactly one gear, changing its tooth count to any integer between 1 and 10⁹. What is the maximum possible greatest common divisor (GCD) of the tooth counts for all N gears after this adjustment?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If the technician re-mills the 7-tooth gear into a 4-tooth gear, the set of gears [4, 6, 8] has a GCD of 2. This is the best possible outcome.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

The technician can choose to "re-mill" a gear to have the same number of teeth it started with.

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
