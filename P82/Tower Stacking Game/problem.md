## Title
Tower Stacking Game

## Slug
tower-stacking-game

## Difficulty
Easy

## Description
A child has n blocks of different widths lined up. They want to build a tower by picking blocks in order, but a block can only be placed on top if it is strictly wider than the one below it (inverted tower).

You have n blocks arranged in a line.
A valid tower consists of blocks chosen in order such that each block is strictly wider than the previous one.

You must choose blocks to find the longest possible inverted tower. You can skip any number of blocks to form the sequence, but you must maintain the original original order of the selected blocks. Calculate the maximum number of blocks that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest inverted towers (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 block.

## Input Format
- The first line contains an integer n: the number of blocks.
- The second line contains n integers x_1, x_2 ... x_n: the width of each block in order.

## Output Format
- Return one integer: the length of the longest valid inverted tower.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
