## Title
Village Alliances

## Slug
village-alliances

## Difficulty
Hard

## Description
There are n villages in a valley. Dirt roads connect some of them. An ancient treaty brings peace only to alliances with a 'Sacred Size'—numbers with digits 4 and 7.

A diplomat wants to build new roads to unite alliances. Merging k alliances requires building k - 1 new roads.

Your task is to determine the minimum number of extra roads the diplomat needs to build to create at least one alliance whose size is a Sacred Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect village 4 with village 3. We can also connect 4 with 1 or 2. This creates a alliance of size 4 (a Sacred Size).

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
There is no way to connect the villages to form a alliance with a size equal to a Sacred Size.

## Input Format
- The first line contains two integers n and m: the number of villages and the number of existing roads.
- The next m lines each contain two integers u and v, representing a road between village u and village v. Note that u may be equal to v, and there may be multiple roads connecting the same pair of villages.

## Output Format
- Return a single integer: the minimum number of roads to build. If no solution exists, print -1.

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
