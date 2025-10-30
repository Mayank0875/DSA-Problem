## Title

Potion Blending

## Slug

potion-blending

## Difficulty

Medium

## Description

You are blending a potion using N ingredients. Each ingredient `i` has `A[i]` units of "magic essence". The potion's stability depends on the greatest common divisor (GCD) of the essence units of all ingredients. You are allowed to substitute exactly one ingredient with a "catalyst" which can have any essence value from 1 to 10⁹. What is the maximum stability (GCD) you can achieve?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

By substituting the ingredient with 7 units for a catalyst with 4 units, the new essence values are [4, 6, 8], which have a GCD of 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

You can use a catalyst with 100 units to replace an ingredient that already has 100 units.

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