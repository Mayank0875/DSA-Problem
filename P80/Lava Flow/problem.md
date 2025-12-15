## Title
Lava Flow

## Slug
lava-flow

## Difficulty
Medium

## Description
A volcano erupted at the Peak (node 1) and lava flows toward the Town (node n).

The mountain consists of $n$ ridges connected by $m$ two-way gullies.
The lava is attempting to travel from the Peak (node 1) to the Town (node $n$).

To prevent this, you can divert specific gullies. Blocking a gully diverts the lava.

Your task is to calculate the **minimum number of gullies** that must be blocked to completely sever all routes between the Peak and the Town.

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
We can divert edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of ridges and gullies.
- The next $m$ lines describe the gullies. Each line contains two integers $a$ and $b$, indicating a gully between ridge $a$ and ridge $b$.

## Output Format
- Return one integer: the minimum number of gullies that need to be blocked.

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
