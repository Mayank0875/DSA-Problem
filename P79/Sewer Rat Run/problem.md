## Title
Sewer Rat Run

## Slug
sewer-rat-run

## Difficulty
Medium

## Description
Rats swim through pipes. Water levels rise and flood the pipe after disturbance.

The sewer consists of $n$ drains and $m$ one-way pipes. Each pipe connects a specific source drain to a destination drain.

The process happens over several rats. In each rat, you must send a rat from drain 1 (the source) to drain $n$ (the destination). The catch is that each pipe floods and becomes impassable. This means each pipe can be used at most once across all rats combined.

Your goal is to determine the maximum number of rats you can successfully complete the journey from drain 1 to drain $n$.

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
You can complete 2 rats.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 rat.

## Input Format
- The first line contains two integers $n$ and $m$: the number of drains and the number of pipes.
- The next $m$ lines describe the pipes. Each line contains two integers $a$ and $b$, indicating a directed pipe from drain $a$ to drain $b$.

## Output Format
- Return one integer: the maximum number of rats possible.

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
