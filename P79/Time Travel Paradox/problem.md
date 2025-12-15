## Title
Time Travel Paradox

## Slug
time-travel-paradox

## Difficulty
Medium

## Description
Travelers jump timelines. A timeline destabilizes and vanishes after one jump.

The multiverse consists of $n$ eras and $m$ one-way portals. Each portal connects a specific source era to a destination era.

The process happens over several travelers. In each traveler, you must send a traveler from era 1 (the source) to era $n$ (the destination). The catch is that each portal destabilizes the timeline, closing the portal. This means each portal can be used at most once across all travelers combined.

Your goal is to determine the maximum number of travelers you can successfully complete the journey from era 1 to era $n$.

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
You can complete 2 travelers.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 traveler.

## Input Format
- The first line contains two integers $n$ and $m$: the number of eras and the number of portals.
- The next $m$ lines describe the portals. Each line contains two integers $a$ and $b$, indicating a directed portal from era $a$ to era $b$.

## Output Format
- Return one integer: the maximum number of travelers possible.

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
