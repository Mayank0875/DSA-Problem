## Title
Beehive Construction

## Slug
beehive-construction

## Difficulty
Hard

## Description
A bee adds cells to a comb. It can build a single cell or a double cell structure.

The bee starts at cell 0 and wishes to reach cell $n$. On each move, The bee can build forward either **1 cell** or **2 cells**.

Your task is to calculate the total number of distinct ways to reach exactly cell $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach cell 2:
1. 1 cell + 1 cell
2. 2 cells

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
- The only input line has an integer $n$ — the target cell.

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

