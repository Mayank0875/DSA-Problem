## Title
Dungeon Crawler

## Slug
dungeon-crawler

## Difficulty
Medium

## Description
A monster spawns in the Pit (node 1) and hunts the Hero at the Exit (node n).

The dungeon consists of $n$ rooms connected by $m$ two-way doors.
The monster is attempting to travel from the Pit (node 1) to the Hero (node $n$).

To prevent this, you can lock specific doors. Locking a door stops the monster.

Your task is to calculate the **minimum number of doors** that must be locked to completely sever all routes between the Pit and the Hero.

## Examples

### 1

#### Input
4 5
1 2
1 3
2 3
3 4
1 4

#### Output
2

#### Explanation
The minimum is 2.

### 2

#### Input
3 3
1 2
2 3
1 3

#### Output
2

#### Explanation
We can lock edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of rooms and doors.
- The next $m$ lines describe the doors. Each line contains two integers $a$ and $b$, indicating a door between room $a$ and room $b$.

## Output Format
- Return one integer: the minimum number of doors that need to be locked.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
