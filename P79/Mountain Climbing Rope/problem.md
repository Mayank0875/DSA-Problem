## Title
Mountain Climbing Rope

## Slug
mountain-climbing-rope

## Difficulty
Medium

## Description
Climbers ascend fixed lines. Old ropes fray and snap after bearing weight once.

The peak consists of $n$ ledges and $m$ one-way ropes. Each rope connects a specific source ledge to a destination ledge.

The process happens over several climbers. In each climber, you must send a climber from ledge 1 (the source) to ledge $n$ (the destination). The catch is that each rope frays and snaps after supporting one person. This means each rope can be used at most once across all climbers combined.

Your goal is to determine the maximum number of climbers you can successfully complete the journey from ledge 1 to ledge $n$.

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
You can complete 2 climbers.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 climber.

## Input Format
- The first line contains two integers $n$ and $m$: the number of ledges and the number of ropes.
- The next $m$ lines describe the ropes. Each line contains two integers $a$ and $b$, indicating a directed rope from ledge $a$ to ledge $b$.

## Output Format
- Return one integer: the maximum number of climbers possible.

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
