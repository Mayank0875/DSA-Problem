## Title

Balanced Bracket Checker

## Slug

balanced-bracket-checker

## Difficulty

Easy

## Description

You are developing a tool to check the syntax of code snippets. A crucial part is ensuring that brackets like parentheses (), square brackets [], and curly braces {} are correctly balanced and nested. A sequence of brackets is considered valid if:
    1. Every opening bracket has a corresponding closing bracket of the same type.
    2. Brackets are closed in the correct order (no crossing pairs like ([)]). An empty string is also considered valid. 
Given a string consisting only of these bracket characters, determine if it is valid.

## Examples

### 1

#### Input

()[]{}

#### Output

Yes

#### Explanation

All brackets are matched correctly.
    
### 2

#### Input

([)]

#### Output

No

#### Explanation
The square bracket [ is closed by a parenthesis ) before the parenthesis ( is closed. This violates the nesting order.
  

## Input Format  

- A single line containing a string s consisting only of the characters '(', ')', '{', '}', '[' and ']'

## Output Format  

- Return true if the string is valid, and false otherwise.
  

## Constraints  

- 1 ≤ length(s) ≤ 1e5
- s contains only parentheses '()', square brackets '[]', and curly braces '{}'.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, string