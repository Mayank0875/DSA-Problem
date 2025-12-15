## Title
Firefighter Stairwell

## Slug
firefighter-stairwell

## Difficulty
Medium

## Description
Firefighters ascend a burning tower. Weak stairs collapse after a team climbs them.

The tower consists of $n$ floors and $m$ one-way stairs. Each staircase connects a specific source floor to a destination floor.

The process happens over several teams. In each team, you must send a team from floor 1 (the source) to floor $n$ (the destination). The catch is that each staircase collapses due to fire damage after use. This means each staircase can be used at most once across all teams combined.

Your goal is to determine the maximum number of teams you can successfully complete the journey from floor 1 to floor $n$.

## Examples

### 1

#### Input
6 7
1 2
1 3
2 6
3 4
3 5
4 6
5 6

#### Output
2

#### Explanation
You can complete 2 teams.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 team.

## Input Format
- The first line contains two integers $n$ and $m$: the number of floors and the number of stairs.
- The next $m$ lines describe the stairs. Each line contains two integers $a$ and $b$, indicating a directed staircase from floor $a$ to floor $b$.

## Output Format
- Return one integer: the maximum number of teams possible.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
