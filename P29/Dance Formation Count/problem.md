## Title

Dance Formation Count

## Slug

dance-formation-count

## Difficulty

Easy

## Description

A dance involves $n$ 'Step-In' moves and $n$ 'Step-Out' moves. A 'graceful' performance requires that the sequence of moves is balanced: every 'Step-In' has a corresponding 'Step-Out', and the dancers never 'Step-Out' unless they have already 'Stepped-In'. How many different 'graceful' dance sequences are possible?
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