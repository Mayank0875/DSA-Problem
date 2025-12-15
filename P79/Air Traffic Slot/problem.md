## Title
Air Traffic Slot

## Slug
air-traffic-slot

## Difficulty
Medium

## Description
Planes fly through sectors. Airspace slots are booked and closed for safety intervals.

The sky consists of $n$ beacons and $m$ one-way airways. Each airway connects a specific source beacon to a destination beacon.

The process happens over several planes. In each plane, you must send a plane from beacon 1 (the source) to beacon $n$ (the destination). The catch is that each airway is closed for a safety interval. This means each airway can be used at most once across all planes combined.

Your goal is to determine the maximum number of planes you can successfully complete the journey from beacon 1 to beacon $n$.

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
You can complete 2 planes.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 plane.

## Input Format
- The first line contains two integers $n$ and $m$: the number of beacons and the number of airways.
- The next $m$ lines describe the airways. Each line contains two integers $a$ and $b$, indicating a directed airway from beacon $a$ to beacon $b$.

## Output Format
- Return one integer: the maximum number of planes possible.

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
