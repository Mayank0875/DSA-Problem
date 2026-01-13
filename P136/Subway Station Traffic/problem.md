## Title
Subway Station Traffic

## Slug
subway-station-traffic

## Difficulty
Medium

## Description
A commuter travels through a city. The passenger volume at a station is the product of its line and stop numbers.

The subway map is represented as an $n \times n$ grid. The passenger volume in the cell at the $i$-th row and $j$-th column is $i \cdot j$ (using 1-based indexing). The commuter starts at position $(1, 1)$ and must reach $(n, n)$.

The commuter can only move **Right** (from $(i, j)$ to $(i, j+1)$) or **Down** (from $(i, j)$ to $(i+1, j)$). Stepping outside the grid is not allowed.

Your task is to calculate the maximum total passenger volume The commuter can encounter on the path, including the starting and ending cells.

Return the result multiplied by $2022$, modulo $10^9 + 7$.
*(Note: Perform the multiplication by 2022 before taking the modulo).*

## Examples

### 1

#### Input
2

#### Output
14154

#### Explanation
For $n=2$, the grid is:
[1, 2]
[2, 4]
Possible paths:
1. (1,1) -> (1,2) -> (2,2). Sum = $1 + 2 + 4 = 7$.
2. (1,1) -> (2,1) -> (2,2). Sum = $1 + 2 + 4 = 7$.
Max sum is 7.
Result = $7 \times 2022 = 14154$.

### 2

#### Input
3

#### Output
44484

#### Explanation
Max path sum for $n=3$ is 22.
$22 \times 2022 = 44484$.

## Input Format
- The only input line has an integer $n$.

## Output Format
- Return one integer: the maximum weighted sum modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, math, matrix
