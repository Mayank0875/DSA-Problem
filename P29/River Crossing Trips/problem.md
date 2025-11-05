## Title

River Crossing Trips

## Slug

river-crossing-trips

## Difficulty

Easy

## Description

A single boat ferries people across a river. It can make $n$ trips 'East' (from A to B) and $n$ trips 'West' (from B to A). The boat starts on the West bank (A). A 'valid' schedule is a sequence of trips that never tries to go 'East' if the boat is already on the East bank, and always ends back at the West bank. How many valid schedules exist?
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