## Title
Bee Nectar Gathering

## Slug
bee-nectar-gathering

## Difficulty
Medium

## Description
Bees visit flowers. A flower is drained of nectar after one visit.

The garden consists of $n$ plants and $m$ one-way paths. Each path connects a specific source plant to a destination plant.

The process happens over several bees. In each bee, you must send a bee from plant 1 (the source) to plant $n$ (the destination). The catch is that each path is drained of all nectar. This means each path can be used at most once across all bees combined.

Your goal is to determine the maximum number of bees you can successfully complete the journey from plant 1 to plant $n$.

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
You can complete 2 bees.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 bee.

## Input Format
- The first line contains two integers $n$ and $m$: the number of plants and the number of paths.
- The next $m$ lines describe the paths. Each line contains two integers $a$ and $b$, indicating a directed path from plant $a$ to plant $b$.

## Output Format
- Return one integer: the maximum number of bees possible.

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
