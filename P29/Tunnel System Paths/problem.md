## Title

Tunnel System Paths

## Slug

tunnel-system-paths

## Difficulty

Easy

## Description

You are exploring a tunnel system. There are $n$ 'descend' (go deeper) shafts and $n$ 'ascend' (go up) shafts. A 'valid path' is a sequence of these shafts that starts at the surface, never goes *above* the surface (you can't ascend if you're already at the top), and ends back at the surface. How many different valid paths are there?
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