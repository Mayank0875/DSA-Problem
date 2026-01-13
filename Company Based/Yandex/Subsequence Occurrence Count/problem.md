## Title

Subsequence Occurrence Count

## Slug

subsequence-occurrence-count

## Difficulty

Medium

## Description

You are given two strings $s$ and $t$ consisting of lowercase English letters.

Your task is to count the number of distinct ways to form the string $s$ as a subsequence of $t$.

A string $s$ is a subsequence of $t$ if it can be obtained by deleting zero or more characters from $t$ without changing the relative order of the remaining characters.

Two ways are considered distinct if the sets of indices of the characters chosen from $t$ are different. Since the answer may be very large, return it modulo $10^9 + 7$.

## Examples

### 1

#### Input

bag
babgbag

#### Output

5

#### Explanation

The string "bag" can be formed from "babgbag" in 5 distinct ways.
Indices in $t$ (0-indexed):
1. [0, 1, 3]
2. [0, 1, 6]
3. [0, 5, 6]
4. [2, 5, 6]
5. [4, 5, 6]
    
### 2

#### Input

rabbbit
rabbit

#### Output

3

#### Explanation

There are 3 ways to form "rabbit" from "rabbbit" (by choosing 2 out of the 3 'b's).

## Input Format  

- The first line contains the string $s$.
- The second line contains the string $t$.

## Output Format  

- Return a single integer — the number of distinct subsequences modulo $10^9 + 7$.
  

## Constraints  

- 1 ≤ s.length ≤ 100
- 1 ≤ t.length ≤ 1e4
- $s$ and $t$ consist of lowercase English letters.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

string, dynamic-programming

## Company
yandex