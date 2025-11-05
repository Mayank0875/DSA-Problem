## Title

Message Acknowledgment

## Slug

message-acknowledgment

## Difficulty

Easy

## Description

A network protocol sends $n$ 'SEND' packets and expects $n$ 'ACK' (acknowledgment) packets. A 'reliable' communication stream is one where every 'SEND' is eventually followed by an 'ACK', and an 'ACK' is never received before its corresponding 'SEND'. How many different reliable communication streams can be formed?
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