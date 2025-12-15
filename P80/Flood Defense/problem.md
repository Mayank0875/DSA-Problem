## Title
Flood Defense

## Slug
flood-defense

## Difficulty
Medium

## Description
The river has overflowed at the Levee (node 1) and water is rushing toward the Hospital (node n).

The drainage system consists of $n$ basins connected by $m$ two-way canals.
The floodwater is attempting to travel from the Levee (node 1) to the Hospital (node $n$).

To prevent this, you can block specific canals. Blocking a canal stops the water.

Your task is to calculate the **minimum number of canals** that must be blocked to completely sever all routes between the Levee and the Hospital.

## Examples

### 1

#### Input
4 5
1 2
1 3
2 3
3 4
1 4

#### Output
2

#### Explanation
The minimum is 2.

### 2

#### Input
3 3
1 2
2 3
1 3

#### Output
2

#### Explanation
We can block edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of basins and canals.
- The next $m$ lines describe the canals. Each line contains two integers $a$ and $b$, indicating a canal between basin $a$ and basin $b$.

## Output Format
- Return one integer: the minimum number of canals that need to be blocked.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
