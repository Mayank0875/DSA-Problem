## Title
Wind Farm

## Slug
wind-farm

## Difficulty
Hard

## Description
n turbines are in a field. Cables connect some into grids. The operator wants grids of 'Power Number' (digits 4 and 7).

You can lay cables. Merging k grids requires k - 1 cables.

Your task is to determine the minimum number of extra cables the operator needs to build to create at least one grid whose size is a Power Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect turbine 4 with turbine 3. We can also connect 4 with 1 or 2. This creates a grid of size 4 (a Power Number).

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
There is no way to connect the turbines to form a grid with a size equal to a Power Number.

## Input Format
- The first line contains two integers n and m: the number of turbines and the number of existing cables.
- The next m lines each contain two integers u and v, representing a cable between turbine u and turbine v. Note that u may be equal to v, and there may be multiple cables connecting the same pair of turbines.

## Output Format
- Return a single integer: the minimum number of cables to build. If no solution exists, print -1.

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
