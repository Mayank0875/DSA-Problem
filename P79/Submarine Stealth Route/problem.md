## Title
Submarine Stealth Route

## Slug
submarine-stealth-route

## Difficulty
Medium

## Description
Subs sneak past sensors. A route is detected and closed after one sub uses it.

The ocean sector consists of $n$ waypoints and $m$ one-way channels. Each channel connects a specific source waypoint to a destination waypoint.

The process happens over several subs. In each sub, you must send a submarine from waypoint 1 (the source) to waypoint $n$ (the destination). The catch is that each channel is compromised by enemy sonar after passage. This means each channel can be used at most once across all subs combined.

Your goal is to determine the maximum number of subs you can successfully complete the journey from waypoint 1 to waypoint $n$.

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
You can complete 2 subs.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 sub.

## Input Format
- The first line contains two integers $n$ and $m$: the number of waypoints and the number of channels.
- The next $m$ lines describe the channels. Each line contains two integers $a$ and $b$, indicating a directed channel from waypoint $a$ to waypoint $b$.

## Output Format
- Return one integer: the maximum number of subs possible.

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
