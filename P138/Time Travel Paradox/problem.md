## Title
Time Travel Paradox

## Slug
time-travel-paradox

## Difficulty
Medium

## Description
A traveler from year $x$ visits year $y$. A paradox is avoided if the timeline divergence (XOR) divides the year.

The traveler defines a specific relationship between a fixed integer $x$ and a candidate integer $y$. A value $y$ is considered "**safe**" with $x$ if:
1. $y$ is a positive integer such that $1 \le y \le m$.
2. $y \neq x$.
3. The value $k = (x \oplus y)$ satisfies: **$k$ divides $x$** OR **$k$ divides $y$**.

Here, $\oplus$ denotes the bitwise XOR operation. An integer $a$ divides $b$ if $b \% a == 0$.

Given the fixed value $x$ and the upper bound $m$, your task is to count the total number of safe integers $y$.

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
- Return a single integer representing the count of safe values.

## Constraints
- 1 ≤ x ≤ 10^6
- 1 ≤ m ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
math, number-theory

