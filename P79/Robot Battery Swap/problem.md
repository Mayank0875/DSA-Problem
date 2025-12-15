## Title
Robot Battery Swap

## Slug
robot-battery-swap

## Difficulty
Medium

## Description
Robots travel between charging pads. Cables fuse after one high-voltage charge transfer.

The factory floor consists of $n$ pads and $m$ one-way cables. Each cable connects a specific source pad to a destination pad.

The process happens over several robots. In each robot, you must send a robot from pad 1 (the source) to pad $n$ (the destination). The catch is that each cable fuses and breaks after a single use. This means each cable can be used at most once across all robots combined.

Your goal is to determine the maximum number of robots you can successfully complete the journey from pad 1 to pad $n$.

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
You can complete 2 robots.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 robot.

## Input Format
- The first line contains two integers $n$ and $m$: the number of pads and the number of cables.
- The next $m$ lines describe the cables. Each line contains two integers $a$ and $b$, indicating a directed cable from pad $a$ to pad $b$.

## Output Format
- Return one integer: the maximum number of robots possible.

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
