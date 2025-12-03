## Title
Apartment Complex

## Slug
apartment-complex

## Difficulty
Hard

## Description
n buildings are in a complex. Skybridges connect some into blocks. The landlord wants blocks of 'Rent Size' (digits 4 and 7).

You can build skybridges. Merging k blocks requires k - 1 bridges.

Your task is to determine the minimum number of extra bridges the landlord needs to build to create at least one block whose size is a Rent Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect building 4 with building 3. We can also connect 4 with 1 or 2. This creates a block of size 4 (a Rent Size).

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
There is no way to connect the buildings to form a block with a size equal to a Rent Size.

## Input Format
- The first line contains two integers n and m: the number of buildings and the number of existing bridges.
- The next m lines each contain two integers u and v, representing a skybridge between building u and building v. Note that u may be equal to v, and there may be multiple bridges connecting the same pair of buildings.

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
