## Title

Balanced Substring Check

## Slug

balanced-substring-check

## Difficulty

Easy

## Description

While not directly about palindromes, we are examining a property of binary strings. We define a "balanced substring" as a contiguous part of the string containing an equal number of '0's and '1's. Your task is to analyze a given binary string and find the length of its longest balanced substring. This property is sometimes used in string analysis algorithms.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The substring "01" is the longest balanced substring.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

"01" and "10" are the longest balanced substrings.

## Input Format

- The first line contains a single integer N, the length of the binary string (represented as an array).
- The second line contains N space-separated integers (0 or 1), representing the string.

## Output Format

- Return a single integer representing the length of the longest contiguous balanced substring.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, strings, prefix sum, hashmap