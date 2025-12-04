## Title
Interplanetary Trade Blocs

## Slug
interplanetary-trade-blocs

## Difficulty
Medium

## Description
In a galaxy, N planets are connected by M one-way wormholes. A Trade Bloc is defined as a set of planets where merchants can travel from any planet in the set to any other and return.

Two planets a and b belong to the same Trade Bloc if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of wormholes.
In other words, two planets are in the same Trade Bloc if they are mutually reachable.

Your task is to: Determine how many Trade Blocs exist in total.

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
The planets form two distinct groups where round-trip traversal is possible within each group.
Planets {1, 2, 3} form one Trade Bloc.
Path: 1 -> 2 -> 3 -> 1.
Planets {4, 5} form another Trade Bloc.
Path: 4 -> 5 -> 4.
Total Trade Blocs: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 planets and 1 one-way wormhole.
Wormhole: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Trade Blocs.

## Input Format
- The first line contains two integers n and m: the number of planets and wormholes.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way wormhole from planet a to planet b.

## Output Format
- Return one integer: the total number of Trade Blocs.

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
