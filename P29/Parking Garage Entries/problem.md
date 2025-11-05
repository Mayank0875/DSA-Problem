## Title

Parking Garage Entries

## Slug

parking-garage-entries

## Difficulty

Easy

## Description

A parking garage is tracking its usage. Over a day, $n$ cars 'Enter' and $n$ cars 'Exit'. A 'valid' sequence of events means that an 'Exit' can only happen if a car is already inside (the number of 'Enter' events is greater than 'Exit' events). How many different valid sequences of $n$ entries and $n$ exits are there, assuming the garage starts and ends empty?
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