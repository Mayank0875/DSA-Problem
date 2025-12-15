## Title
Satellite Relay Battery

## Slug
satellite-relay-battery

## Difficulty
Medium

## Description
Satellites beam data. On-board capacitors discharge fully after one transmission.

The orbit consists of $n$ satellites and $m$ one-way beams. Each beam connects a specific source satellite to a destination satellite.

The process happens over several signals. In each signal, you must send a signal from satellite 1 (the source) to satellite $n$ (the destination). The catch is that each beam drains the capacitor banks completely. This means each beam can be used at most once across all signals combined.

Your goal is to determine the maximum number of signals you can successfully complete the journey from satellite 1 to satellite $n$.

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
You can complete 2 signals.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 signal.

## Input Format
- The first line contains two integers $n$ and $m$: the number of satellites and the number of beams.
- The next $m$ lines describe the beams. Each line contains two integers $a$ and $b$, indicating a directed beam from satellite $a$ to satellite $b$.

## Output Format
- Return one integer: the maximum number of signals possible.

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
