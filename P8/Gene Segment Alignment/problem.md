## Title

Gene Segment Alignment

## Slug

gene-segment-alignment

## Difficulty

Medium

## Description

A biologist is studying a DNA strand composed of N gene segments. Each segment `i` has a length `A[i]`. The biologist believes the segments are related if their lengths share a large common divisor. They can use gene editing to replace exactly one segment with a new segment of any length from 1 to 10⁹. What is the maximum possible greatest common divisor (GCD) of all N segment lengths after this edit?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

By replacing the segment of length 7 with one of length 4, the lengths become [4, 6, 8]. The GCD of these is 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

The biologist can "edit" a segment to be the same length it was before.

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