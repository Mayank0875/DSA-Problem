## Title

Balanced Transaction Log

## Slug

balanced-transaction-log

## Difficulty

Easy

## Description

A financial transaction log contains $n$ 'credit' entries and $n$ 'debit' entries. The log is 'balanced' if, when read in order, the account balance never goes negative and ends at zero. (Assume 1 credit = +1, 1 debit = -1). How many different balanced sequences of $n$ credits and $n$ debits are there?
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