## Title

Server Request Sequencing

## Slug

server-request-sequencing

## Difficulty

Easy

## Description

A server receives $n$ 'START' requests and $n$ 'END' requests for a specific task. A sequence of these requests is 'valid' if every 'START' has a corresponding 'END' that comes after it, and at no point have more 'END' requests been processed than 'START' requests. For $n$ pairs, how many different valid sequences of 'START' and 'END' requests are there?
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