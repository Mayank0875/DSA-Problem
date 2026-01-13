## Title
Beehive Construction

## Slug
beehive-construction

## Difficulty
Medium

## Description
A bee connects cell $y$ to cell $x$. The structure holds if the hex-distance (XOR) divides the cell index.

The bee defines a specific relationship between a fixed integer $x$ and a candidate integer $y$. A value $y$ is considered "**connected**" with $x$ if:
1. $y$ is a positive integer such that $1 \le y \le m$.
2. $y \neq x$.
3. The value $k = (x \oplus y)$ satisfies: **$k$ divides $x$** OR **$k$ divides $y$**.

Here, $\oplus$ denotes the bitwise XOR operation. An integer $a$ divides $b$ if $b \% a == 0$.

Given the fixed value $x$ and the upper bound $m$, your task is to count the total number of connected integers $y$.

## Examples

### 1

#### Input
6 9

#### Output
3

#### Explanation
For $x=6, m=9$:
- $y=4$: $x \oplus y = 2$. $2$ divides $6$. Valid.
- $y=5$: $x \oplus y = 3$. $3$ divides $6$. Valid.
- $y=7$: $x \oplus y = 1$. $1$ divides $6$. Valid.
Total valid values: 3.

### 2

#### Input
5 7

#### Output
2

#### Explanation
For $x=5, m=7$:
- $y=4$: $x \oplus y = 1$. $1$ divides $5$. Valid.
- $y=6$: $x \oplus y = 3$. $3$ divides $6$. Valid.
Total valid values: 2.

## Input Format
- A single line containing two space-separated integers $x$ and $m$.

## Output Format
- Return a single integer representing the count of connected values.

## Constraints
- 1 ≤ x ≤ 10^6
- 1 ≤ m ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
math, number-theory

