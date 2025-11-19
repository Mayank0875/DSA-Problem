## Title
Tetris Gap Analysis

## Slug
tetris-gap-analysis

## Difficulty
Medium

## Description
In a game of Tetris, the piled blocks form a jagged landscape. You are analyzing the game state to find the largest rectangular solid area formed by the stacked blocks. This helps in evaluating the stability of the stack. Given the column heights, calculate this maximum rectangular area.

## Examples

### 1

#### Input
7
[6, 2, 5, 4, 5, 1, 6]

#### Output
12

#### Explanation
The largest rectangular area has a height of 4 and spans across elements with heights [5, 4, 5]. The width is 3 units (from index 2 to 4). Area = height * width = 4 * 3 = 12.

### 2

#### Input
4
[2, 1, 5, 6]

#### Output
10

#### Explanation
The largest rectangle has height 5 and spans elements with heights [5, 6]. Width = 2. Area = 5 * 2 = 10.

## Input Format
- The first line contains a single integer n, the number of elements.
- The second line contains n space-separated integers, representing the heights/values of the elements from left to right.

## Output Format
- Return a single integer representing the maximum possible rectangular area.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ height ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, array
