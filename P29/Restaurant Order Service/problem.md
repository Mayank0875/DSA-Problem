## Title

Restaurant Order Service

## Slug

restaurant-order-service

## Difficulty

Easy

## Description

A restaurant is tracking its flow of orders. There are $n$ 'Order In' events and $n$ 'Order Out' (served) events. A 'valid' service sequence means that an 'Order Out' event can only happen if a corresponding 'Order In' event has already occurred. Given $n$ pairs, how many different valid service sequences are there?
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