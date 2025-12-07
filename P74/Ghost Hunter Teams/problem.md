## Title
Ghost Hunter Teams

## Slug
ghost-hunter-teams

## Difficulty
Medium

## Description
Rooms in a haunted mansion are connected. Ghost hunters are stationed in rooms and need to pair up with a hunter in an adjacent room to stay safe.

The structure is a tree with n rooms and n-1 doors.
A team is formed between two rooms connected by a door.
However, each room can be part of at most one team.

Your task is to calculate the maximum number of teams that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of teams is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 teams.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form teams (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of rooms.
- The next n-1 lines each contain two integers u and v, representing a door between room u and room v.

## Output Format
- Return a single integer representing the maximum number of teams.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
