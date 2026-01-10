## Title
The King's Decree

## Slug
the-kings-decree

## Difficulty
Medium

## Description
A mad king demands that all official decrees be palindromes. The royal scribe must edit the current draft with minimal changes.

You are given a string `s` representing the decree text. Your goal is to convert this string into a palindrome (a sequence that reads the same forwards and backwards) to satisfy the king.

In one operation, you can either:
1. **Insert** a letter anywhere in the string.
2. **Delete** a letter from anywhere in the string.

Find the **minimum total number of operations** (insertions plus deletions) required to make the string a palindrome.

## Examples

### 1

#### Input
abc

#### Output
2

#### Explanation
We can delete 'b' and 'c' to get "a" (2 operations).
Alternatively, we could insert 'b' and 'a' to get "abcba" (2 operations).
The minimum is 2.

### 2

#### Input
mbadm

#### Output
2

#### Explanation
We can delete 'b' and 'd' to get "mam" (2 operations).
Or we can insert 'd' and 'b' to get "mbdadbm" (2 operations).
The minimum is 2.

## Input Format
- The first line contains a single string `s`.

## Output Format
- Return a single integer representing the minimum number of operations.

## Constraints
- 1 ≤ s.length ≤ 1000
- `s` consists of lowercase English letters.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, dynamic-programming, longest-common-subsequence

## Company
google, amazon
