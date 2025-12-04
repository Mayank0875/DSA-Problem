## Title
Supply Chain Logistics

## Slug
supply-chain-logistics

## Difficulty
Medium

## Description
Warehouses ship goods on one-way routes. A Logistic Hub is a group of warehouses that can transfer goods to each other.

Two warehouses a and b belong to the same Hub if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of routes.
In other words, two warehouses are in the same Hub if they are mutually reachable.

Your task is to: Determine how many Hubs exist in total.

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
The warehouses form two distinct groups where round-trip traversal is possible within each group.
Warehouses {1, 2, 3} form one Hub.
Path: 1 -> 2 -> 3 -> 1.
Warehouses {4, 5} form another Hub.
Path: 4 -> 5 -> 4.
Total Hubs: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 warehouses and 1 one-way route.
Route: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Hubs.

## Input Format
- The first line contains two integers n and m: the number of warehouses and routes.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way route from warehouse a to warehouse b.

## Output Format
- Return one integer: the total number of Hubs.

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
