## Title
Galactic Trade Routes

## Slug
galactic-trade-routes

## Difficulty
Hard

## Description
A space empire consists of n star systems. Hyperlanes connect some systems. The Emperor follows an ancient prophecy stating that prosperity comes to trade zones containing a 'Divine Number' of systems—integers made only of 4 and 7.

The Emperor orders the construction of new hyperlanes to merge trade zones. Merging k zones requires k - 1 new hyperlanes.

Your task is to determine the minimum number of extra hyperlanes the Emperor needs to build to create at least one trade zone whose size is a Divine Number. If this goal cannot be achieved, return -1.

## Examples

### 1

#### Input
4 3
1 2
2 3
1 3

#### Output
1

#### Explanation
The optimal way is to connect star system 4 with star system 3. We can also connect 4 with 1 or 2. This creates a trade zone of size 4 (a Divine Number).

### 2

#### Input
5 4
1 2
3 4
4 5
3 5

#### Output
-1

#### Explanation
There is no way to connect the star systems to form a trade zone with a size equal to a Divine Number.

## Input Format
- The first line contains two integers n and m: the number of star systems and the number of existing hyperlanes.
- The next m lines each contain two integers u and v, representing a hyperlane between star system u and star system v. Note that u may be equal to v, and there may be multiple hyperlanes connecting the same pair of star systems.

## Output Format
- Return a single integer: the minimum number of hyperlanes to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
