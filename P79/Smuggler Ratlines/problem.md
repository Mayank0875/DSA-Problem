## Title
Smuggler Ratlines

## Slug
smuggler-ratlines

## Difficulty
Medium

## Description
Smugglers move contraband. Patrols shut down a route once suspicious activity is spotted.

The border consists of $n$ hideouts and $m$ one-way paths. Each path connects a specific source hideout to a destination hideout.

The process happens over several runs. In each run, you must send a smuggler from hideout 1 (the source) to hideout $n$ (the destination). The catch is that each path is discovered and closed by authorities. This means each path can be used at most once across all runs combined.

Your goal is to determine the maximum number of runs you can successfully complete the journey from hideout 1 to hideout $n$.

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
You can complete 2 runs.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 run.

## Input Format
- The first line contains two integers $n$ and $m$: the number of hideouts and the number of paths.
- The next $m$ lines describe the paths. Each line contains two integers $a$ and $b$, indicating a directed path from hideout $a$ to hideout $b$.

## Output Format
- Return one integer: the maximum number of runs possible.

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
