## Title
Animal Migration

## Slug
animal-migration

## Difficulty
Medium

## Description
A herd of wild boars moves from the Forest (node 1) to the Highway (node n).

The reserve consists of $n$ clearings connected by $m$ two-way game trails.
The herd is attempting to travel from the Forest (node 1) to the Highway (node $n$).

To prevent this, you can fence specific game trails. Fencing a trail stops the animals.

Your task is to calculate the **minimum number of game trails** that must be fenced to completely sever all routes between the Forest and the Highway.

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
We can fence edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of clearings and game trails.
- The next $m$ lines describe the game trails. Each line contains two integers $a$ and $b$, indicating a game trail between clearing $a$ and clearing $b$.

## Output Format
- Return one integer: the minimum number of game trails that need to be fenced.

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
