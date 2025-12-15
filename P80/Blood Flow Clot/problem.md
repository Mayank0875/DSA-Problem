## Title
Blood Flow Clot

## Slug
blood-flow-clot

## Difficulty
Medium

## Description
A dangerous toxin is in the Artery (node 1) moving to the Heart (node n).

The circulatory system consists of $n$ vessels connected by $m$ two-way veins.
The toxin is attempting to travel from the Artery (node 1) to the Heart (node $n$).

To prevent this, you can clamp specific veins. Clamping a vein stops blood flow.

Your task is to calculate the **minimum number of veins** that must be clamped to completely sever all routes between the Artery and the Heart.

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
We can clamp edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of vessels and veins.
- The next $m$ lines describe the veins. Each line contains two integers $a$ and $b$, indicating a vein between vessel $a$ and vessel $b$.

## Output Format
- Return one integer: the minimum number of veins that need to be clamped.

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
