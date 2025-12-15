## Title
Conveyor Belt Sabotage

## Slug
conveyor-belt-sabotage

## Difficulty
Medium

## Description
Defective parts leave the Mold (node 1) and head to Packaging (node n).

The assembly line consists of $n$ machines connected by $m$ two-way belts.
Defective parts is attempting to travel from the Mold (node 1) to Packaging (node $n$).

To prevent this, you can stop specific belts. Stopping a belt prevents flow.

Your task is to calculate the **minimum number of belts** that must be stopped to completely sever all routes between the Mold and Packaging.

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
We can stop edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of machines and belts.
- The next $m$ lines describe the belts. Each line contains two integers $a$ and $b$, indicating a belt between machine $a$ and machine $b$.

## Output Format
- Return one integer: the minimum number of belts that need to be stopped.

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
