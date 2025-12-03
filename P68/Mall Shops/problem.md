## Title
Mall Shops

## Slug
mall-shops

## Difficulty
Hard

## Description
n shops are in a mall. Hallways connect some into wings. The owner wants wings of 'Retail Size' (digits 4 and 7).

You can open hallways. Merging k wings requires k - 1 renovations.

Your task is to determine the minimum number of extra renovations the owner needs to build to create at least one wing whose size is a Retail Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect shop 4 with shop 3. We can also connect 4 with 1 or 2. This creates a wing of size 4 (a Retail Size).

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
There is no way to connect the shops to form a wing with a size equal to a Retail Size.

## Input Format
- The first line contains two integers n and m: the number of shops and the number of existing renovations.
- The next m lines each contain two integers u and v, representing a hallway between shop u and shop v. Note that u may be equal to v, and there may be multiple renovations connecting the same pair of shops.

## Output Format
- Return a single integer: the minimum number of renovations to build. If no solution exists, print -1.

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
