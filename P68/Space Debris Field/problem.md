## Title
Space Debris Field

## Slug
space-debris-field

## Difficulty
Hard

## Description
n pieces of debris float in orbit. Gravity tethers connect some into junk piles. A scavenger seeks piles of 'Scrap Value' size (digits 4 and 7).

The scavenger can shoot tethers. Merging k piles requires k - 1 tethers.

Your task is to determine the minimum number of extra tethers the scavenger needs to build to create at least one pile whose size is a Scrap Value. If this goal cannot be achieved, return -1.

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
The optimal way is to connect debris piece 4 with debris piece 3. We can also connect 4 with 1 or 2. This creates a pile of size 4 (a Scrap Value).

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
There is no way to connect the pieces to form a pile with a size equal to a Scrap Value.

## Input Format
- The first line contains two integers n and m: the number of pieces and the number of existing tethers.
- The next m lines each contain two integers u and v, representing a tether between debris piece u and debris piece v. Note that u may be equal to v, and there may be multiple tethers connecting the same pair of pieces.

## Output Format
- Return a single integer: the minimum number of tethers to build. If no solution exists, print -1.

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
