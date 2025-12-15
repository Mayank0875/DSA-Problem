## Title
Migrating Birds

## Slug
migrating-birds

## Difficulty
Medium

## Description
Birds fly south. Stopover food sources are depleted after one flock feeds.

The flyway consists of $n$ landmarks and $m$ one-way flight paths. Each flight path connects a specific source landmark to a destination landmark.

The process happens over several flocks. In each flock, you must send a flock from landmark 1 (the source) to landmark $n$ (the destination). The catch is that each flight path runs out of food and cannot support another flock. This means each flight path can be used at most once across all flocks combined.

Your goal is to determine the maximum number of flocks you can successfully complete the journey from landmark 1 to landmark $n$.

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
You can complete 2 flocks.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 flock.

## Input Format
- The first line contains two integers $n$ and $m$: the number of landmarks and the number of flight paths.
- The next $m$ lines describe the flight paths. Each line contains two integers $a$ and $b$, indicating a directed flight path from landmark $a$ to landmark $b$.

## Output Format
- Return one integer: the maximum number of flocks possible.

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
