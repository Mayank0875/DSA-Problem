## Title
Mountain Climber Ropes

## Slug
mountain-climber-ropes

## Difficulty
Medium

## Description
Climbers are securing themselves on a rock face. They pair up with a connected climber to belay. Each climber can belay one person.

The structure is a tree with n climbers and n-1 ropes.
A belay team is formed between two climbers connected by a rope.
However, each climber can be part of at most one belay team.

Your task is to calculate the maximum number of belay teams that can be formed.

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
One optimal set of belay teams is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 belay teams.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form belay teams (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of climbers.
- The next n-1 lines each contain two integers u and v, representing a rope between climber u and climber v.

## Output Format
- Return a single integer representing the maximum number of belay teams.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
