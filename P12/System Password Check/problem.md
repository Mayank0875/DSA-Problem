## Title

System Password Check

## Slug

system-password-check

## Difficulty

Easy

## Description

A high-security system requires a password S to be a palindrome to be valid. A palindrome is a string that is identical when read forwards or backward. Your job is to write the verification module. Given a string S, return 'Yes' if it is a valid (palindromic) password, and 'No' otherwise.

## Examples

### 1

#### Input

level

#### Output

Yes

#### Explanation

The string "level" reads the same forwards and backward.
    
### 2

#### Input

adam

#### Output

No

#### Explanation

The string "adam" does not read the same forwards and backward ("mada").  

## Input Format  

- The input consists of a single line containing a string S.
- The string S contains only lowercase English letters (a - z).

## Output Format  

- Return 'Yes' if S is a palindrome, and 'No' otherwise.
  

## Constraints  

- 1 ≤ length(s) ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

strings, implementation, two-pointers