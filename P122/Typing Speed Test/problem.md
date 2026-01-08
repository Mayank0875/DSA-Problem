## Title
Typing Speed Test

## Slug
typing-speed-test

## Difficulty
Hard

## Description
A typist hits keys. They can type one character or a common bigram (2 chars) macro.

The typist starts at char 0 and wishes to reach char $n$. On each move, The typist can type forward either **1 char** or **2 chars**.

Your task is to calculate the total number of distinct ways to reach exactly char $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach char 2:
1. 1 char + 1 char
2. 2 chars

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
- The only input line has an integer $n$ — the target char.

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

