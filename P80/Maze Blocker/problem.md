## Title
Maze Blocker

## Slug
maze-blocker

## Difficulty
Medium

## Description
A robot mouse is trying to solve a maze from Start (node 1) to Cheese (node n).

The maze consists of $n$ cells connected by $m$ two-way passages.
The mouse is attempting to travel from Start (node 1) to Cheese (node $n$).

To prevent this, you can wall up specific passages. Walling up a passage blocks the mouse.

Your task is to calculate the **minimum number of passages** that must be walled up to completely sever all routes between Start and Cheese.

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
We can wall up edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of cells and passages.
- The next $m$ lines describe the passages. Each line contains two integers $a$ and $b$, indicating a passage between cell $a$ and cell $b$.

## Output Format
- Return one integer: the minimum number of passages that need to be walled up.

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
