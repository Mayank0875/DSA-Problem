## Title
Relay Race Baton

## Slug
relay-race-baton

## Difficulty
Medium

## Description
Runners pass a baton. Runners are exhausted and cannot run a second leg.

The track consists of $n$ zones and $m$ one-way sprints. Each sprint connects a specific source zone to a destination zone.

The process happens over several batons. In each baton, you must send a baton from zone 1 (the source) to zone $n$ (the destination). The catch is that each sprint exhausts the runner assigned to that segment. This means each sprint can be used at most once across all batons combined.

Your goal is to determine the maximum number of batons you can successfully complete the journey from zone 1 to zone $n$.

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
You can complete 2 batons.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 baton.

## Input Format
- The first line contains two integers $n$ and $m$: the number of zones and the number of sprints.
- The next $m$ lines describe the sprints. Each line contains two integers $a$ and $b$, indicating a directed sprint from zone $a$ to zone $b$.

## Output Format
- Return one integer: the maximum number of batons possible.

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
