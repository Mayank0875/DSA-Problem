## Title
Laser Security Grid

## Slug
laser-security-grid

## Difficulty
Medium

## Description
An intruder tries to cross from the Lobby (node 1) to the Elevators (node n) avoiding beams.

The grid consists of $n$ safe spots connected by $m$ two-way paths.
The intruder is attempting to travel from the Lobby (node 1) to the Elevators (node $n$).

To prevent this, you can activate specific paths. Activating a laser on a path blocks it.

Your task is to calculate the **minimum number of paths** that must be activated to completely sever all routes between the Lobby and the Elevators.

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
We can activate edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of safe spots and paths.
- The next $m$ lines describe the paths. Each line contains two integers $a$ and $b$, indicating a path between safe spot $a$ and safe spot $b$.

## Output Format
- Return one integer: the minimum number of paths that need to be activated.

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
