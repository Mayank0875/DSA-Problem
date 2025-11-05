## Title

Gate Open Close Sequences

## Slug

gate-open-close-sequences

## Difficulty

Easy

## Description

A high-security airlock has $n$ 'Open' commands and $n$ 'Close' commands. To maintain pressure, the system must follow a 'safe' sequence. A sequence is 'safe' if the 'Close' command is never sent unless a corresponding 'Open' command was sent first, and all commands are matched. How many safe sequences exist?
## Examples

### 1

#### Input

3

#### Output

5

#### Explanation

The 5 unique well-formed combinations are:
((()))
(()())
(())()
()(())
()()()

### 2

#### Input

1

#### Output

1

#### Explanation
The only combination is ().

## Input Format  

- The input consists of a single line containing one integer, `n`.

## Output Format  

- Return single integer representing total number of well-formed parenthesis combinations.
  

## Constraints  

- 1 ≤ n ≤ 8

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion