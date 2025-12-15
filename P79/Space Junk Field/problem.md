## Title
Space Junk Field

## Slug
space-junk-field

## Difficulty
Medium

## Description
Ships navigate debris. The debris field shifts and closes the gap after a ship passes.

The orbit consists of $n$ sectors and $m$ one-way gaps. Each gap connects a specific source sector to a destination sector.

The process happens over several ships. In each ship, you must send a ship from sector 1 (the source) to sector $n$ (the destination). The catch is that each gap closes up with drifting debris. This means each gap can be used at most once across all ships combined.

Your goal is to determine the maximum number of ships you can successfully complete the journey from sector 1 to sector $n$.

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
You can complete 2 ships.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 ship.

## Input Format
- The first line contains two integers $n$ and $m$: the number of sectors and the number of gaps.
- The next $m$ lines describe the gaps. Each line contains two integers $a$ and $b$, indicating a directed gap from sector $a$ to sector $b$.

## Output Format
- Return one integer: the maximum number of ships possible.

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
