## Title
Mirror Dimension Message

## Slug
mirror-dimension-message

## Difficulty
Medium

## Description
You are trying to send a message through a portal to the Mirror Dimension. The portal only accepts symmetric text strings.

You are given a string `s` representing the message. Your goal is to convert this string into a palindrome (a sequence that reads the same forwards and backwards) to pass it through the portal.

In one operation, you can either:
1. **Insert** a character anywhere in the string.
2. **Delete** a character from anywhere in the string.

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
