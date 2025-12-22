## Title
Broken Telegraph

## Slug
broken-telegraph

## Difficulty
Medium

## Description
A telegraph operator receives a stream `s`. Due to a faulty wire, some signals might have been phantom clicks. The operator needs to list all possible valid signals that could have been sent by ignoring some clicks.

Your task is to determine the total number of distinct non-empty signals that can be formed. Two signals are considered distinct if they are not identical strings. As the number of possibilities can be substantial, print the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
aybabtu

#### Output
103

#### Explanation
The string "aybabtu" contains repeating characters. By removing various characters, we can generate 103 distinct non-empty subsequences.

### 2

#### Input
a

#### Output
1

#### Explanation
The string "a" contains a single character. Only 1 distinct non-empty subsequence exists.

## Input Format
- The first line contains a single string $s$ consisting of lowercase English characters (a–z).

## Output Format
- Return one integer: the number of distinct non-empty strings that can be generated, modulo $10^9 + 7$.

## Constraints
- 1 ≤ s.length ≤ 1e5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, string
