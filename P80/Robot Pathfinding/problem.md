## Title
Robot Pathfinding

## Slug
robot-pathfinding

## Difficulty
Medium

## Description
A malfunctioning robot tries to go from the Charging Dock (node 1) to the Restricted Area (node n).

The factory floor consists of $n$ stations connected by $m$ two-way aisles.
The robot is attempting to travel from the Dock (node 1) to the Restricted Area (node $n$).

To prevent this, you can obstruct specific aisles. Placing an obstacle in an aisle stops the robot.

Your task is to calculate the **minimum number of aisles** that must be obstructed to completely sever all routes between the Dock and the Restricted Area.

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
We can obstruct edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of stations and aisles.
- The next $m$ lines describe the aisles. Each line contains two integers $a$ and $b$, indicating a aisle between station $a$ and station $b$.

## Output Format
- Return one integer: the minimum number of aisles that need to be obstructed.

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
