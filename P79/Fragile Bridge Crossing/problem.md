## Title
Fragile Bridge Crossing

## Slug
fragile-bridge-crossing

## Difficulty
Medium

## Description
An army retreats across a valley of rope bridges. Each bridge snaps after a squad crosses.

The valley consists of $n$ cliffs and $m$ one-way bridges. Each bridge connects a specific source cliff to a destination cliff.

The process happens over several squads. In each squad, you must send a squad from cliff 1 (the source) to cliff $n$ (the destination). The catch is that each bridge snaps under the weight and falls into the abyss. This means each bridge can be used at most once across all squads combined.

Your goal is to determine the maximum number of squads you can successfully complete the journey from cliff 1 to cliff $n$.

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
You can complete 2 squads.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 squad.

## Input Format
- The first line contains two integers $n$ and $m$: the number of cliffs and the number of bridges.
- The next $m$ lines describe the bridges. Each line contains two integers $a$ and $b$, indicating a directed bridge from cliff $a$ to cliff $b$.

## Output Format
- Return one integer: the maximum number of squads possible.

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
