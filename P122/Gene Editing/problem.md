## Title
Gene Editing

## Slug
gene-editing

## Difficulty
Hard

## Description
CRISPR targets a sequence. It can edit 1 base or a 2-base codon.

The tool starts at base 0 and wishes to reach base $n$. On each move, The tool can edit forward either **1 base** or **2 bases**.

Your task is to calculate the total number of distinct ways to reach exactly base $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach base 2:
1. 1 base + 1 base
2. 2 bases

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
- The only input line has an integer $n$ — the target base.

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

