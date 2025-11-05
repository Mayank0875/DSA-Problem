## Title

Theater Ticket Line

## Slug

theater-ticket-line

## Difficulty

Easy

## Description

A theater is selling tickets for 5 dollars. There are $2n$ people in line; $n$ of them have a 5-dollar bill, and $n$ of them have a 10-dollar bill. The ticket seller starts with no change. A sequence of customers is 'valid' if the seller can always provide change for every 10-dollar bill. How many different valid customer sequences are there?
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