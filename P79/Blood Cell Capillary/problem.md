## Title
Blood Cell Capillary

## Slug
blood-cell-capillary

## Difficulty
Medium

## Description
White blood cells squeeze through capillaries. Inflammation blocks the vessel after one passage.

The tissue consists of $n$ junctions and $m$ one-way capillaries. Each capillary connects a specific source junction to a destination junction.

The process happens over several cells. In each cell, you must send a cell from junction 1 (the source) to junction $n$ (the destination). The catch is that each capillary swells and closes up after a cell squeezes through. This means each capillary can be used at most once across all cells combined.

Your goal is to determine the maximum number of cells you can successfully complete the journey from junction 1 to junction $n$.

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
You can complete 2 cells.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 cell.

## Input Format
- The first line contains two integers $n$ and $m$: the number of junctions and the number of capillaries.
- The next $m$ lines describe the capillaries. Each line contains two integers $a$ and $b$, indicating a directed capillary from junction $a$ to junction $b$.

## Output Format
- Return one integer: the maximum number of cells possible.

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
