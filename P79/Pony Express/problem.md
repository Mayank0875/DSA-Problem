## Title
Pony Express

## Slug
pony-express

## Difficulty
Medium

## Description
Riders carry mail. Horses on a route are exhausted after one gallop.

The trail map consists of $n$ outposts and $m$ one-way segments. Each segment connects a specific source outpost to a destination outpost.

The process happens over several riders. In each rider, you must send a rider from outpost 1 (the source) to outpost $n$ (the destination). The catch is that each segment exhausts the horses stationed there for the season. This means each segment can be used at most once across all riders combined.

Your goal is to determine the maximum number of riders you can successfully complete the journey from outpost 1 to outpost $n$.

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
You can complete 2 riders.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 rider.

## Input Format
- The first line contains two integers $n$ and $m$: the number of outposts and the number of segments.
- The next $m$ lines describe the segments. Each line contains two integers $a$ and $b$, indicating a directed segment from outpost $a$ to outpost $b$.

## Output Format
- Return one integer: the maximum number of riders possible.

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
