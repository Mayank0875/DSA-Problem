## Title
Dungeon Rooms

## Slug
dungeon-rooms

## Difficulty
Hard

## Description
n rooms are in a dungeon. Passages connect some into levels. The hero wants levels of 'Quest Size' (digits 4 and 7).

You can dig passages. Merging k levels requires k - 1 digs.

Your task is to determine the minimum number of extra digs the hero needs to build to create at least one level whose size is a Quest Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect room 4 with room 3. We can also connect 4 with 1 or 2. This creates a level of size 4 (a Quest Size).

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
There is no way to connect the rooms to form a level with a size equal to a Quest Size.

## Input Format
- The first line contains two integers n and m: the number of rooms and the number of existing digs.
- The next m lines each contain two integers u and v, representing a passage between room u and room v. Note that u may be equal to v, and there may be multiple digs connecting the same pair of rooms.

## Output Format
- Return a single integer: the minimum number of digs to build. If no solution exists, print -1.

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
