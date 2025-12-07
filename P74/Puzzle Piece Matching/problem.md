## Title
Puzzle Piece Matching

## Slug
puzzle-piece-matching

## Difficulty
Medium

## Description
Puzzle pieces are spread out but connected by fit. You assemble them in pairs first. Each piece connects to one other.

The structure is a tree with n pieces and n-1 fits.
A assembled pair is formed between two pieces connected by a fit.
However, each piece can be part of at most one assembled pair.

Your task is to calculate the maximum number of assembled pairs that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of assembled pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 assembled pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form assembled pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of pieces.
- The next n-1 lines each contain two integers u and v, representing a fit between piece u and piece v.

## Output Format
- Return a single integer representing the maximum number of assembled pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
