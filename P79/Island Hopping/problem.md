## Title
Island Hopping

## Slug
island-hopping

## Difficulty
Medium

## Description
Refugees flee via small boats. Boats are abandoned or sink after one crossing.

The archipelago consists of $n$ islands and $m$ one-way crossings. Each crossing connects a specific source island to a destination island.

The process happens over several groups. In each group, you must send a group from island 1 (the source) to island $n$ (the destination). The catch is that each crossing uses up the available fuel or boat. This means each crossing can be used at most once across all groups combined.

Your goal is to determine the maximum number of groups you can successfully complete the journey from island 1 to island $n$.

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
You can complete 2 groups.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 group.

## Input Format
- The first line contains two integers $n$ and $m$: the number of islands and the number of crossings.
- The next $m$ lines describe the crossings. Each line contains two integers $a$ and $b$, indicating a directed crossing from island $a$ to island $b$.

## Output Format
- Return one integer: the maximum number of groups possible.

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
