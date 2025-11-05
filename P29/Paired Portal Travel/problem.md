## Title

Paired Portal Travel

## Slug

paired-portal-travel

## Difficulty

Easy

## Description

A dimension traveler uses portals. There are $n$ 'Entry' portals and $n$ 'Exit' portals. A 'safe journey' is a sequence of portal uses where every 'Entry' is matched by a later 'Exit', and the traveler never 'Exits' a dimension they haven't 'Entered'. How many different safe journey sequences can be made?
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