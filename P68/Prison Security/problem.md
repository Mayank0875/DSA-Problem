## Title
Prison Security

## Slug
prison-security

## Difficulty
Hard

## Description
n cells are in a prison. Corridors connect some into wings. The warden wants wings of 'Guard Size' (digits 4 and 7).

You can unlock doors. Merging k wings requires unlocking k - 1 doors.

Your task is to determine the minimum number of extra unlocks the warden needs to build to create at least one wing whose size is a Guard Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect cell 4 with cell 3. We can also connect 4 with 1 or 2. This creates a wing of size 4 (a Guard Size).

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
There is no way to connect the cells to form a wing with a size equal to a Guard Size.

## Input Format
- The first line contains two integers n and m: the number of cells and the number of existing unlocks.
- The next m lines each contain two integers u and v, representing a corridor between cell u and cell v. Note that u may be equal to v, and there may be multiple unlocks connecting the same pair of cells.

## Output Format
- Return a single integer: the minimum number of unlocks to build. If no solution exists, print -1.

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
