## Title
Warehouse Bin Consolidation

## Slug
warehouse-bin-consolidation

## Difficulty
Medium

## Description
Bins are connected by conveyors. Workers consolidate contents of adjacent bins into one crate. Each bin is emptied once.

The structure is a tree with n bins and n-1 conveyors.
A consolidation is formed between two bins connected by a conveyor.
However, each bin can be part of at most one consolidation.

Your task is to calculate the maximum number of consolidations that can be formed.

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
One optimal set of consolidations is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 consolidations.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form consolidations (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of bins.
- The next n-1 lines each contain two integers u and v, representing a conveyor between bin u and bin v.

## Output Format
- Return a single integer representing the maximum number of consolidations.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
