## Title
Crowd Control Barriers

## Slug
crowd-control-barriers

## Difficulty
Medium

## Description
Fans rush the stage. Security barriers break under the pressure of a crowd surge.

The stadium consists of $n$ zones and $m$ one-way gates. Each gate connects a specific source zone to a destination zone.

The process happens over several surges. In each surge, you must send a crowd wave from zone 1 (the source) to zone $n$ (the destination). The catch is that each gate breaks under the pressure. This means each gate can be used at most once across all surges combined.

Your goal is to determine the maximum number of surges you can successfully complete the journey from zone 1 to zone $n$.

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
- The first line contains two integers $n$ and $m$: the number of zones and the number of gates.
- The next $m$ lines describe the gates. Each line contains two integers $a$ and $b$, indicating a directed gate from zone $a$ to zone $b$.

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
