## Title
Philosophical Arguments

## Slug
philosophical-arguments

## Difficulty
Medium

## Description
Arguments lead to conclusions (other arguments). A School of Thought is a set of arguments that support each other.

Two arguments a and b belong to the same School if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of implications.
In other words, two arguments are in the same School if they are mutually reachable.

Your task is to: Determine how many Schools exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The arguments form two distinct groups where round-trip traversal is possible within each group.
Arguments {1, 2, 3} form one School.
Path: 1 -> 2 -> 3 -> 1.
Arguments {4, 5} form another School.
Path: 4 -> 5 -> 4.
Total Schools: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 arguments and 1 one-way implication.
Implication: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Schools.

## Input Format
- The first line contains two integers n and m: the number of arguments and implications.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way implication from argument a to argument b.

## Output Format
- Return one integer: the total number of Schools.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
