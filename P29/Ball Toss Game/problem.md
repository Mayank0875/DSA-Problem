## Title

Ball Toss Game

## Slug

ball-toss-game

## Difficulty

Easy

## Description

In a game, there are $n$ 'Throw' actions and $n$ 'Catch' actions. A 'valid' game sequence must be well-formed: every 'Throw' must be followed by a 'Catch', and a 'Catch' can only happen after a 'Throw' has occurred. You must find the total number of different valid game sequences.
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