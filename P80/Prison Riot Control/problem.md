## Title
Prison Riot Control

## Slug
prison-riot-control

## Difficulty
Medium

## Description
A riot started in Cell Block A (node 1) and prisoners are trying to reach the Armory (node n).

The prison consists of $n$ rooms connected by $m$ two-way corridors.
The mob is attempting to travel from Cell Block A (node 1) to the Armory (node $n$).

To prevent this, you can lock down specific corridors. Locking down a corridor prevents movement.

Your task is to calculate the **minimum number of corridors** that must be locked down to completely sever all routes between Cell Block A and the Armory.

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
We can lock down edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of rooms and corridors.
- The next $m$ lines describe the corridors. Each line contains two integers $a$ and $b$, indicating a corridor between room $a$ and room $b$.

## Output Format
- Return one integer: the minimum number of corridors that need to be locked down.

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
