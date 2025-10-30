## Title

Orbital Resonance

## Slug

orbital-resonance

## Difficulty

Medium

## Description

An astronomer is observing N planets. Each planet `i` has an orbital period of `A[i]` days. The astronomer suspects a resonance, which is strongest when the periods share a large common divisor. They have a theory that one planet is an anomaly. If they could change the orbital period of exactly one planet to any value between 1 and 10⁹, what is the maximum possible GCD of all N periods?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If the planet with a 7-day period actually had a 4-day period, the periods [4, 6, 8] would have a GCD of 2. This is the maximum resonance.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

Changing one planet's period to 100 (which it already is) is a valid move.

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