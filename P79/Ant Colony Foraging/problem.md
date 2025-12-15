## Title
Ant Colony Foraging

## Slug
ant-colony-foraging

## Difficulty
Medium

## Description
Ants carry food from a source to the nest. Pheromone trails evaporate instantly after use.

The colony consists of $n$ chambers and $m$ one-way tunnels. Each tunnel connects a specific source chamber to a destination chamber.

The process happens over several trips. In each trip, you must send a ant from chamber 1 (the source) to chamber $n$ (the destination). The catch is that each tunnel collapses due to loose soil after an ant passes. This means each tunnel can be used at most once across all trips combined.

Your goal is to determine the maximum number of trips you can successfully complete the journey from chamber 1 to chamber $n$.

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
You can complete 2 trips.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 trip.

## Input Format
- The first line contains two integers $n$ and $m$: the number of chambers and the number of tunnels.
- The next $m$ lines describe the tunnels. Each line contains two integers $a$ and $b$, indicating a directed tunnel from chamber $a$ to chamber $b$.

## Output Format
- Return one integer: the maximum number of trips possible.

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
