## Title
Electric Grid Fuse

## Slug
electric-grid-fuse

## Difficulty
Medium

## Description
Power surges travel to ground. Fuses blow to protect the system after passing current.

The grid consists of $n$ breakers and $m$ one-way wires. Each wire connects a specific source breaker to a destination breaker.

The process happens over several surges. In each surge, you must send a surge from breaker 1 (the source) to breaker $n$ (the destination). The catch is that each wire blows its fuse and cuts the connection. This means each wire can be used at most once across all surges combined.

Your goal is to determine the maximum number of surges you can successfully complete the journey from breaker 1 to breaker $n$.

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
You can complete 2 surges.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 surge.

## Input Format
- The first line contains two integers $n$ and $m$: the number of breakers and the number of wires.
- The next $m$ lines describe the wires. Each line contains two integers $a$ and $b$, indicating a directed wire from breaker $a$ to breaker $b$.

## Output Format
- Return one integer: the maximum number of surges possible.

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
