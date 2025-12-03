## Title
Forest Root Systems

## Slug
forest-root-systems

## Difficulty
Hard

## Description
n trees stand in a forest. Roots connect some into groves. The Druids protect groves with a 'Nature Number' of trees (digits 4 and 7).

You can graft roots to merge groves. Merging k groves takes k - 1 grafts.

Your task is to determine the minimum number of extra grafts the druid needs to build to create at least one grove whose size is a Nature Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect tree 4 with tree 3. We can also connect 4 with 1 or 2. This creates a grove of size 4 (a Nature Number).

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
There is no way to connect the trees to form a grove with a size equal to a Nature Number.

## Input Format
- The first line contains two integers n and m: the number of trees and the number of existing grafts.
- The next m lines each contain two integers u and v, representing a root between tree u and tree v. Note that u may be equal to v, and there may be multiple grafts connecting the same pair of trees.

## Output Format
- Return a single integer: the minimum number of grafts to build. If no solution exists, print -1.

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
