## Title

Ancient Rune Alignment

## Slug

ancient-rune-alignment

## Difficulty

Medium

## Description

A sealed door has N ancient runes arranged in a circle. Each rune `i` has a power level `A[i]`. To open the door, all runes must "resonate" at a common frequency, which must be a common divisor of their power levels. You have a special "artificer's hammer" that can re-carve exactly one rune, changing its power level to any integer from 1 to 10⁹. What is the maximum resonance frequency (GCD) you can achieve?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If you re-carve the rune with power 7 to have power 4, the runes [4, 6, 8] will all resonate at frequency 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

You can re-carve a rune to have the same power level it already has.

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