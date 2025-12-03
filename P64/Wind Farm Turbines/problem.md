## Title
Wind Farm Turbines

## Slug
wind-farm-turbines

## Difficulty
Medium

## Description
N wind turbines are offshore. Maintenance boats travel between them. A boat has fuel for a round trip of squared distance X. Find the minimum fuel capacity X to allow travel between all turbines.

Your task is to find the minimum integer value of X (squared distance limit) that ensures every turbine can communicate/connect with every other turbine, either directly or through a chain of intermediates.

## Examples

### 1

#### Input
4
1 3
5 4
7 2
6 1

#### Output
17

#### Explanation
The optimal strategy connects the turbines using links whose squared distances are at most 17.
For example, the squared distance between the points (1,3) and (5,4) is:
(1 - 5)² + (3 - 4)² = 16 + 1 = 17.
If the turbines can connect up to a squared distance of 17, the network becomes fully connected.

### 2

#### Input
3
0 0
0 10
10 0

#### Output
100

#### Explanation
We need to connect (0,0) to either (0,10) or (10,0). Both points are at a squared distance of 100 from the origin.
A squared distance of 100 is enough to form the path:
(0,10) <-> (0,0) <-> (10,0).

## Input Format
- The first line contains an integer N, the number of turbines.
- The next N lines each contain two integers x and y, representing the coordinates of a turbine.

## Output Format
- Return a single integer X, the minimum fuel capacity required to connect the network.

## Constraints
- 1 ≤ N ≤ 1000
- 1 ≤ x, y ≤ 25000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, binary-search
