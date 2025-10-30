## Title

Tidy Garden

## Slug

tidy-garden

## Difficulty

Medium

## Description

A gardener has N plants in a row, with heights `A[1], ..., A[N]`. The gardener wants to make the garden look tidy. Tidiness is measured by the greatest common divisor (GCD) of all plant heights. The gardener has one replacement plant, which can be grown to any height between 1 and 10⁹ (inclusive). They will swap this new plant with exactly one of the existing N plants. What is the maximum possible tidiness (GCD) they can achieve?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If the gardener replaces the plant of height 7 with a new plant of height 4, the heights become [4, 6, 8]. The GCD of these is 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

The gardener can replace a plant of height 100 with a new plant of height 100.

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