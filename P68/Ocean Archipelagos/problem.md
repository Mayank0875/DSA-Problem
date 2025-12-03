## Title
Ocean Archipelagos

## Slug
ocean-archipelagos

## Difficulty
Hard

## Description
The ocean has n tiny islets. Shallow reefs connect some into atolls. A legendary treasure is buried in an atoll with a 'Golden Size' (digits 4 and 7).

A pirate can build bridges to merge atolls. Merging k atolls requires k - 1 bridges.

Your task is to determine the minimum number of extra bridges the pirate needs to build to create at least one atoll whose size is a Golden Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect islet 4 with islet 3. We can also connect 4 with 1 or 2. This creates a atoll of size 4 (a Golden Size).

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
There is no way to connect the islets to form a atoll with a size equal to a Golden Size.

## Input Format
- The first line contains two integers n and m: the number of islets and the number of existing bridges.
- The next m lines each contain two integers u and v, representing a reef between islet u and islet v. Note that u may be equal to v, and there may be multiple bridges connecting the same pair of islets.

## Output Format
- Return a single integer: the minimum number of bridges to build. If no solution exists, print -1.

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
