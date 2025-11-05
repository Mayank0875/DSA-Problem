## Title

Train Shunting Sequences

## Slug

train-shunting-sequences

## Difficulty

Easy

## Description

You are a train yard operator with $n$ cars to shunt. You can perform $n$ 'Siding' (push a car in) operations and $n$ 'Mainline' (pull a car out) operations. Cars exit the siding in LIFO order (like a stack). A 'valid' sequence of operations ensures you never pull from an empty siding. How many valid sequences of $n$ 'Siding' and $n$ 'Mainline' ops are there?
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