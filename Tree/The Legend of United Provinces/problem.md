## Title

The Legend of United Provinces

## Slug

the-legend-of-united-provinces

## Difficulty

Easy

## Description

In the ancient land of Algora, there are $n$ mysterious cities. Some cities share direct trade routes, while others are isolated. Due to the "Transitive Alliance" law, if city $A$ connects to city $B$, and city $B$ connects to city $C$, then city $A$ is indirectly connected to city $C$. A province is defined as a maximum group of cities where every city is reachable from any other city within the group, either directly or indirectly. No city outside a province can be connected to any city inside it. You are given an $n \times n$ matrix, isConnected, representing the map of Algora. If isConnected[i][j] = 1, the $i^{th}$ and $j^{th}$ cities are directly connected. Your task is to count the total number of distinct provinces in the land.

## Examples

### 1

#### Input

[[1,1,0],[1,1,0],[0,0,1]]

#### Output

2

#### Explanation

Cities 1 and 2 are connected to each other, forming the first province. City 3 is isolated, forming the second province.
    
### 2

#### Input

[[1,0,0],[0,1,0],[0,0,1]]

#### Output

3

#### Explanation

No cities are connected to each other. Each city forms its own independent province.
  

## Input Format  

- The input consists of an $n \times n$ adjacency matrix isConnected
- The matrix represents connections between $n$ cities.

## Output Format  

- Return a single integer representing the total number of provinces found.
  

## Constraints  

- 1 ≤ n ≤ 100
- isConnected[i][j] is $1$ or $0$. 
- isConnected[i][i] == 1 (Each city is connected to itself).
- isConnected[i][j] == isConnected[j][i] (Connections are bidirectional).

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph, depth-first-search, breadth-first-search