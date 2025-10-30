## Title

Robot Command Sequence

## Slug

robot-command-sequence

## Difficulty

Easy

## Description

A robot is given a command sequence S. For the command to be executed correctly, the sequence must be "symmetric," which is defined as being a palindrome. A palindrome string reads the same forwards as it does backward. Does the given command S meet this requirement? Return 'Yes' or 'No'.

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