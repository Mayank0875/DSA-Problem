## Title
Hacker Decryption

## Slug
hacker-decryption

## Difficulty
Medium

## Description
A hacker is breaking a firewall with encryption strength `n`. They can reduce the strength by running scripts that target specific digit values in the current strength code.

You start with a **encryption strength** of `n`. The goal is to reduce this encryption strength to exactly 0.

In one **hack attempt**, you can look at the digits of the current encryption strength, choose one **non-zero digit**, and subtract it from the current encryption strength.

For example, if the encryption strength is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of hack attempts required to reduce the encryption strength to 0.

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
Total hack attempts: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The encryption strength is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of hack attempts.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
