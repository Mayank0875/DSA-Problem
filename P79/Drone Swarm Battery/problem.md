## Title
Drone Swarm Battery

## Slug
drone-swarm-battery

## Difficulty
Medium

## Description
Drones fly point-to-point. Flight consumes the entire battery charge for that leg.

The airspace consists of $n$ waypoints and $m$ one-way legs. Each leg connects a specific source waypoint to a destination waypoint.

The process happens over several drones. In each drone, you must send a drone from waypoint 1 (the source) to waypoint $n$ (the destination). The catch is that each leg consumes the entire battery charge. This means each leg can be used at most once across all drones combined.

Your goal is to determine the maximum number of drones you can successfully complete the journey from waypoint 1 to waypoint $n$.

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
You can complete 2 drones.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 drone.

## Input Format
- The first line contains two integers $n$ and $m$: the number of waypoints and the number of legs.
- The next $m$ lines describe the legs. Each line contains two integers $a$ and $b$, indicating a directed leg from waypoint $a$ to waypoint $b$.

## Output Format
- Return one integer: the maximum number of drones possible.

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
