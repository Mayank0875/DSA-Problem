## Title
Solar Panel Wiring

## Slug
solar-panel-wiring

## Difficulty
Medium

## Description
Solar panels on a roof are connected. Electricians wire them in series pairs to boost voltage. Each panel is part of one pair.

The structure is a tree with n panels and n-1 wires.
A series pair is formed between two panels connected by a wire.
However, each panel can be part of at most one series pair.

Your task is to calculate the maximum number of series pairs that can be formed.

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
One optimal set of series pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 series pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form series pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of panels.
- The next n-1 lines each contain two integers u and v, representing a wire between panel u and panel v.

## Output Format
- Return a single integer representing the maximum number of series pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
