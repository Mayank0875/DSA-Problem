## Title

Building Block Tower

## Slug

building-block-tower

## Difficulty

Medium

## Description

You are building a tower with N blocks, stacked vertically. Each block `i` has a weight `A[i]`. To ensure stability, all block weights should be multiples of a common base weight. You have one "special" block you can use. You must swap this special block with exactly one of the N blocks in the tower. The special block can be assigned any weight from 1 to 10⁹. What is the maximum possible base weight (GCD) of the new tower?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If you swap the 7-weight block with a 4-weight special block, the tower's weights are [4, 6, 8]. The GCD is 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

You can swap a 100-weight block with a special block that also weighs 100.

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