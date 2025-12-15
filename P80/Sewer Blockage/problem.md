## Title
Sewer Blockage

## Slug
sewer-blockage

## Difficulty
Medium

## Description
Pollutants enter at the Factory Drain (node 1) and flow to the Ocean Outlet (node n).

The sewer system consists of $n$ junctions connected by $m$ two-way sewer lines.
The pollutants is attempting to travel from the Factory (node 1) to the Ocean (node $n$).

To prevent this, you can dam specific sewer lines. Damming a line stops the pollution.

Your task is to calculate the **minimum number of sewer lines** that must be dammed to completely sever all routes between the Factory and the Ocean.

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
We can dam edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of junctions and sewer lines.
- The next $m$ lines describe the sewer lines. Each line contains two integers $a$ and $b$, indicating a sewer line between junction $a$ and junction $b$.

## Output Format
- Return one integer: the minimum number of sewer lines that need to be dammed.

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
