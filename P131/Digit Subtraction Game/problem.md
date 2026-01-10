## Title
Digit Subtraction Game

## Slug
digit-subtraction-game

## Difficulty
Medium

## Description
You are playing a mathematical game involving number reduction.

You start with a **value** of `n`. The goal is to reduce this value to exactly 0.

In one **move**, you can look at the digits of the current value, choose one **non-zero digit**, and subtract it from the current value.

For example, if the value is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of moves required to reduce the value to 0.

## Examples

### 1

#### Input
27

#### Output
5

#### Explanation
1. 27 - 7 = 20
2. 20 - 2 = 18
3. 18 - 8 = 10
4. 10 - 1 = 9
5. 9 - 9 = 0
Total moves: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The value is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of moves.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
