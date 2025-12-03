## Title
Theme Park Queues

## Slug
theme-park-queues

## Difficulty
Hard

## Description
n attractions are in a park. Paths connect some into zones. The owner wants zones with a 'Fun Number' of rides (digits 4 and 7).

You can pave new paths. Merging k zones costs k - 1 paths.

Your task is to determine the minimum number of extra paths the owner needs to build to create at least one zone whose size is a Fun Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect attraction 4 with attraction 3. We can also connect 4 with 1 or 2. This creates a zone of size 4 (a Fun Number).

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
There is no way to connect the attractions to form a zone with a size equal to a Fun Number.

## Input Format
- The first line contains two integers n and m: the number of attractions and the number of existing paths.
- The next m lines each contain two integers u and v, representing a path between attraction u and attraction v. Note that u may be equal to v, and there may be multiple paths connecting the same pair of attractions.

## Output Format
- Return a single integer: the minimum number of paths to build. If no solution exists, print -1.

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
