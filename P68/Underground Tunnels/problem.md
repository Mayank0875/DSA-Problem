## Title
Underground Tunnels

## Slug
underground-tunnels

## Difficulty
Hard

## Description
Subterranean gnomes live in n caves. Tunnels connect some caves into colonies. The Gnome King seeks a colony of 'Royal Size' (digits 4 and 7).

Miners can dig new tunnels to connect colonies. Merging k colonies costs k - 1 digging operations.

Your task is to determine the minimum number of extra tunnels the King needs to build to create at least one colony whose size is a Royal Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect cave 4 with cave 3. We can also connect 4 with 1 or 2. This creates a colony of size 4 (a Royal Size).

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
There is no way to connect the caves to form a colony with a size equal to a Royal Size.

## Input Format
- The first line contains two integers n and m: the number of caves and the number of existing tunnels.
- The next m lines each contain two integers u and v, representing a tunnel between cave u and cave v. Note that u may be equal to v, and there may be multiple tunnels connecting the same pair of caves.

## Output Format
- Return a single integer: the minimum number of tunnels to build. If no solution exists, print -1.

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
