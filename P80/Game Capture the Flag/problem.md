## Title
Game Capture the Flag

## Slug
game-capture-the-flag

## Difficulty
Medium

## Description
The enemy Runner (node 1) has the flag and is running to their Base (node n).

The map consists of $n$ zones connected by $m$ two-way paths.
The Runner is attempting to travel from the Flag Point (node 1) to the Enemy Base (node $n$).

To prevent this, you can trap specific paths. Placing a trap on a path stops the runner.

Your task is to calculate the **minimum number of paths** that must be trapped to completely sever all routes between the Flag Point and the Enemy Base.

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
We can trap edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of zones and paths.
- The next $m$ lines describe the paths. Each line contains two integers $a$ and $b$, indicating a path between zone $a$ and zone $b$.

## Output Format
- Return one integer: the minimum number of paths that need to be trapped.

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
