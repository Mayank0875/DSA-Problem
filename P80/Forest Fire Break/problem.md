## Title
Forest Fire Break

## Slug
forest-fire-break

## Difficulty
Medium

## Description
A fire started at the Campsite (node 1) and is spreading toward the Village (node n).

The forest consists of $n$ groves connected by $m$ two-way trails.
The fire is attempting to travel from the Campsite (node 1) to the Village (node $n$).

To prevent this, you can clear specific trails. Clearing a trail creates a firebreak.

Your task is to calculate the **minimum number of trails** that must be cleared to completely sever all routes between the Campsite and the Village.

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
We can clear edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of groves and trails.
- The next $m$ lines describe the trails. Each line contains two integers $a$ and $b$, indicating a trail between grove $a$ and grove $b$.

## Output Format
- Return one integer: the minimum number of trails that need to be cleared.

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
