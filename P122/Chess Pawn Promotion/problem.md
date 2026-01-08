## Title
Chess Pawn Promotion

## Slug
chess-pawn-promotion

## Difficulty
Hard

## Description
In a variant chess game, a pawn races to the end. It can move forward 1 square or dash forward 2 squares.

The pawn starts at rank 0 and wishes to reach rank $n$. On each move, The pawn can move forward either **1 square** or **2 squares**.

Your task is to calculate the total number of distinct ways to reach exactly rank $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach rank 2:
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

