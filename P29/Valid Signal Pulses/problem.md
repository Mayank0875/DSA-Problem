## Title

Valid Signal Pulses

## Slug

valid-signal-pulses

## Difficulty

Easy

## Description

A communication system uses $n$ 'positive' pulses and $n$ 'negative' pulses. A 'valid message' is a sequence of these pulses where the signal's net charge never drops below zero and ends at zero. This ensures every positive pulse is eventually balanced by a negative one. How many different valid messages can be sent?
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