## Title
Wildfire Firebreak

## Slug
wildfire-firebreak

## Difficulty
Medium

## Description
A fire burns in the North Woods (node 1) and wind blows it toward the South Woods (node n).

The woodland consists of $n$ sectors connected by $m$ two-way canopy bridges.
The fire is attempting to travel from North Woods (node 1) to South Woods (node $n$).

To prevent this, you can fell specific canopy bridges. Felling trees breaks the canopy bridge.

Your task is to calculate the **minimum number of canopy bridges** that must be felled to completely sever all routes between North Woods and South Woods.

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
We can fell edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of sectors and canopy bridges.
- The next $m$ lines describe the canopy bridges. Each line contains two integers $a$ and $b$, indicating a canopy bridge between sector $a$ and sector $b$.

## Output Format
- Return one integer: the minimum number of canopy bridges that need to be felled.

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
