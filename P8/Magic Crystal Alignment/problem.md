## Title

Magic Crystal Alignment

## Slug

magic-crystal-alignment

## Difficulty

Medium

## Description

A wizard has N magic crystals in a line, with power levels `A[1], A[2], ..., A[N]`. To activate an ancient device, the power levels must share a high common resonance. The wizard can replace exactly one crystal with a new one, which can have any power level from 1 to 10⁹. Your task is to find the maximum possible "resonance frequency" (the greatest common divisor) of all crystal power levels after the replacement.

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If the wizard replaces the crystal with power 7 with a new crystal of power 4, the levels become [4, 6, 8]. The GCD of these is 2, which is the maximum.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

The wizard can replace a crystal with a new one of the same power.

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