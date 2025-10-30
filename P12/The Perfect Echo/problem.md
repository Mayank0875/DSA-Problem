## Title

The Perfect Echo

## Slug

the-perfect-echo

## Difficulty

Easy

## Description

You are in a mythical canyon. When you shout a word S, the canyon echoes it back. The echo is considered "perfect" if the word S is a palindrome, meaning it reads the same forwards as it does backward. Check if the shouted word S will produce a perfect echo. Return 'Yes' if it's a palindrome, and 'No' otherwise.

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