## Title

File Open Close Pairs

## Slug

file-open-close-pairs

## Difficulty

Easy

## Description

An operating system is tracking file handles. There are $n$ 'open file' operations and $n$ 'close file' operations. A 'safe' sequence of operations ensures that no file is 'closed' before it is 'opened', and all 'open' operations are eventually 'closed'. How many different safe sequences of $n$ open/close pairs are possible?
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