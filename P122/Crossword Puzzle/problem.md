## Title
Crossword Puzzle

## Slug
crossword-puzzle

## Difficulty
Hard

## Description
A solver fills squares. They can fill 1 letter or a known 2-letter word.

The solver starts at square 0 and wishes to reach square $n$. On each move, The solver can fill forward either **1 square** or **2 squares**.

Your task is to calculate the total number of distinct ways to reach exactly square $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach square 2:
1. 1 square + 1 square
2. 2 squares

### 2

#### Input
3

#### Output
3

#### Explanation
There are three ways:
1. 1 + 1 + 1
2. 1 + 2
3. 2 + 1

## Input Format
- The only input line has an integer $n$ — the target square.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

