## Title
Elevator Emergency

## Slug
elevator-emergency

## Difficulty
Medium

## Description
People escape a building. Emergency brakes engage and lock the car after one trip.

The skyscraper consists of $n$ floors and $m$ one-way shafts. Each shaft connects a specific source floor to a destination floor.

The process happens over several groups. In each group, you must send a group from floor 1 (the source) to floor $n$ (the destination). The catch is that each shaft locks the emergency brakes permanently. This means each shaft can be used at most once across all groups combined.

Your goal is to determine the maximum number of groups you can successfully complete the journey from floor 1 to floor $n$.

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
You can complete 2 groups.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 group.

## Input Format
- The first line contains two integers $n$ and $m$: the number of floors and the number of shafts.
- The next $m$ lines describe the shafts. Each line contains two integers $a$ and $b$, indicating a directed shaft from floor $a$ to floor $b$.

## Output Format
- Return one integer: the maximum number of groups possible.

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
