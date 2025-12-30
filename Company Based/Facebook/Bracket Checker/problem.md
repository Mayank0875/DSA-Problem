## Title

Bracket Checker

## Slug

bracket-checker

## Difficulty

Easy

## Description

A computer science student has typed a long string of brackets into a text editor. The string `s` is guaranteed to be a "balanced bracket sequence" (a valid mathematical expression of brackets).

However, the student's keyboard is malfunctioning. When they try to edit the text, the backspace key deletes exactly two characters: one opening bracket `(` and one closing bracket `)`. These two characters can be located anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to delete such that the remaining string is **no longer** a balanced bracket sequence.

## Examples

### 1

#### Input

(())

#### Output

No

#### Explanation

The string is `(())`.
- Removing the outer pair leaves `()`, which is balanced.
- Removing the first `(` and last `)` leaves `()`, balanced.
It is impossible to make it unbalanced.
    
### 2

#### Input

()()

#### Output

Yes

#### Explanation

The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a balanced bracket sequence.  

## Input Format  

- A single line containing a string s consisting only of the characters '(', ')'.

## Output Format  

- Return Yes if it is possible to make the string unbalanced and No otherwise.
  
## Constraints  

- 1 ≤ length(s) ≤ 1e5
- s contains only parentheses '()'.
- The input string `s` is guaranteed to be a balanced bracket sequence.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, string

## Company
facebook