## Title
Water Pipe Burst

## Slug
water-pipe-burst

## Difficulty
Medium

## Description
High pressure water is routed to a tank. Old pipes burst after a single surge.

The plumbing system consists of $n$ junctions and $m$ one-way pipes. Each pipe connects a specific source junction to a destination junction.

The process happens over several surges. In each surge, you must send a flow surge from junction 1 (the source) to junction $n$ (the destination). The catch is that each pipe bursts permanently after carrying one surge. This means each pipe can be used at most once across all surges combined.

Your goal is to determine the maximum number of surges you can successfully complete the journey from junction 1 to junction $n$.

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
- The first line contains two integers $n$ and $m$: the number of junctions and the number of pipes.
- The next $m$ lines describe the pipes. Each line contains two integers $a$ and $b$, indicating a directed pipe from junction $a$ to junction $b$.

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
