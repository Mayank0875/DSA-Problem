## Title
Domino Tiling

## Slug
domino-tiling

## Difficulty
Hard

## Description
You are tiling a $2 	imes n$ grid with $2 	imes 1$ dominoes. You can place one vertical domino (1 unit width) or two horizontal dominoes (2 units width).

The tiler starts at column 0 and wishes to reach column $n$. On each move, The tiler can tile forward either **1 column** or **2 columns**.

Your task is to calculate the total number of distinct ways to reach exactly column $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach column 2:
1. 1 column + 1 column
2. 2 columns

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
- The only input line has an integer $n$ — the target column.

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

