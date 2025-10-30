## Title

Symmetric Star Pattern

## Slug

symmetric-star-pattern

## Difficulty

Easy

## Description

An astronomer records a sequence of star brightness levels as a string S. The pattern is "symmetric" if the string S is a palindrome. A palindrome is a string that reads the same forwards as backward. Is the observed pattern symmetric? Return 'Yes' or 'No'.

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