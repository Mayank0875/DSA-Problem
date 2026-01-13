## Title

Traffic Flow Reorientation

## Slug

traffic-flow-reorientation

## Difficulty

Medium

## Description

There are $n$ cities numbered from $1$ to $n$, connected by $n-1$ roads. The road network forms a tree structure (there is exactly one path between any two cities). Currently, all roads are one-way.

The Ministry of Transport wants to organize a major event in the capital, which is **City 1**. To ensure success, every other city must be able to reach City 1 by traveling along the roads in the correct direction.

You are given the current orientation of the roads. Your task is to determine the **minimum** number of roads that need to be reoriented (have their direction reversed) so that every city can reach City 1.

## Examples

### 1

#### Input

6
1 2
2 4
3 2
5 1
5 6

#### Output

3

#### Explanation

The capital is City 1.
- Road 1->2 points away from 1. Needs flip.
- Road 2->4 points away from 1. Needs flip.
- Road 3->2 points towards 2 (and effectively towards 1). OK.
- Road 5->1 points towards 1. OK.
- Road 5->6 points away from 1 (via 5). Needs flip.
Total flips: 3.
    
### 2

#### Input

5
2 1
2 3
4 3
4 5

#### Output

2

#### Explanation

Roads 2->3 and 4->5 need to be flipped.

## Input Format  

- The first line contains an integer $n$ — the number of cities.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way road from city $u$ to city $v$.

## Output Format  

- Return a single integer representing the minimum number of edges that need to be changed.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ u, v ≤ n
- The graph is guaranteed to be a tree.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

tree, depth-first-search, breadth-first-search

## Company
grab