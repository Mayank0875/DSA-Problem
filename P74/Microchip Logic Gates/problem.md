## Title
Microchip Logic Gates

## Slug
microchip-logic-gates

## Difficulty
Medium

## Description
Logic gates are wired in a tree. Engineers are optimizing the layout by grouping adjacent gates into functional blocks (pairs).

The structure is a tree with n gates and n-1 wires.
A block is formed between two gates connected by a wire.
However, each gate can be part of at most one block.

Your task is to calculate the maximum number of blocks that can be formed.

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
One optimal set of blocks is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 blocks.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form blocks (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of gates.
- The next n-1 lines each contain two integers u and v, representing a wire between gate u and gate v.

## Output Format
- Return a single integer representing the maximum number of blocks.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
