## Title
Racing Cheat

## Slug
racing-cheat

## Difficulty
Medium

## Description
A cheater tries to take shortcuts from Start (node 1) to Finish (node n).

The track consists of $n$ checkpoints connected by $m$ two-way shortcuts.
The cheater is attempting to travel from Start (node 1) to Finish (node $n$).

To prevent this, you can barricade specific shortcuts. Barricading a shortcut forces fair play.

Your task is to calculate the **minimum number of shortcuts** that must be barricaded to completely sever all routes between Start and Finish.

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
We can barricade edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of checkpoints and shortcuts.
- The next $m$ lines describe the shortcuts. Each line contains two integers $a$ and $b$, indicating a shortcut between checkpoint $a$ and checkpoint $b$.

## Output Format
- Return one integer: the minimum number of shortcuts that need to be barricaded.

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
