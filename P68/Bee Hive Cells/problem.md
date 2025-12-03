## Title
Bee Hive Cells

## Slug
bee-hive-cells

## Difficulty
Hard

## Description
n cells are in a hive. Wax walls connect some into combs. The queen wants combs of 'Honey Count' (digits 4 and 7).

Worker bees can build walls. Merging k combs costs k - 1 walls.

Your task is to determine the minimum number of extra walls the worker bee needs to build to create at least one comb whose size is a Honey Count. If this goal cannot be achieved, return -1.

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
The optimal way is to connect cell 4 with cell 3. We can also connect 4 with 1 or 2. This creates a comb of size 4 (a Honey Count).

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
There is no way to connect the cells to form a comb with a size equal to a Honey Count.

## Input Format
- The first line contains two integers n and m: the number of cells and the number of existing walls.
- The next m lines each contain two integers u and v, representing a wall between cell u and cell v. Note that u may be equal to v, and there may be multiple walls connecting the same pair of cells.

## Output Format
- Return a single integer: the minimum number of walls to build. If no solution exists, print -1.

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
