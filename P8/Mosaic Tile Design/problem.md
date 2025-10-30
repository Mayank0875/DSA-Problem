## Title

Mosaic Tile Design

## Slug

mosaic-tile-design

## Difficulty

Medium

## Description

You are designing a mosaic using N tiles, with side lengths `A[1], ..., A[N]`. The design looks best if all tile sizes are multiples of a common "base unit". You have one extra tile and can swap it with exactly one of the N tiles. This extra tile can be cut to any size from 1 to 10⁹. What is the maximum possible "base unit" (greatest common divisor) for the N tiles in the final design?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If you swap the tile of size 7 with a new tile of size 4, the tiles [4, 6, 8] all share a base unit of 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

You can swap a tile with a new one of the exact same size.

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