## Title
Pest Control

## Slug
pest-control

## Difficulty
Medium

## Description
Rats are moving from the Sewer (node 1) to the Restaurant (node n).

The building foundation consists of $n$ crawlspaces connected by $m$ two-way holes.
The rats is attempting to travel from the Sewer (node 1) to the Restaurant (node $n$).

To prevent this, you can patch specific holes. Patching a hole stops the rats.

Your task is to calculate the **minimum number of holes** that must be patched to completely sever all routes between the Sewer and the Restaurant.

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
We can patch edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of crawlspaces and holes.
- The next $m$ lines describe the holes. Each line contains two integers $a$ and $b$, indicating a hole between crawlspace $a$ and crawlspace $b$.

## Output Format
- Return one integer: the minimum number of holes that need to be patched.

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
