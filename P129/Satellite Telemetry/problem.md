## Title
Satellite Telemetry

## Slug
satellite-telemetry

## Difficulty
Medium

## Description
Ground control parses a data stream for a handshake protocol sequence.

You are given two strings `target` and `source` consisting of status bits.

Your task is to count the number of distinct ways to form the string `target` as a subsequence of `source`.

A string `target` is a subsequence of `source` if it can be obtained by deleting zero or more characters from `source` without changing the relative order of the remaining characters.

Two ways are considered distinct if the sets of indices of the characters chosen from `source` are different. Since the answer may be very large, return it modulo $10^9 + 7$.

## Examples

### 1

#### Input
bag
babgbag

#### Output
5

#### Explanation
The string "bag" can be formed from "babgbag" in 5 distinct ways.
Indices in `source` (0-indexed):
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
There are 3 ways to form "rabbit" from "rabbbit" (by choosing different 'b's).

## Input Format
- The first line contains the string `target`.
- The second line contains the string `source`.

## Output Format
- Return a single integer — the number of distinct subsequences modulo $10^9 + 7$.

## Constraints
- 1 ≤ target.length ≤ 1000
- 1 ≤ source.length ≤ 1000
- Strings consist of status bits.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, dynamic-programming

## Company
google, amazon
