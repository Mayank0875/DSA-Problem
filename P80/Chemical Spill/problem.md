## Title
Chemical Spill

## Slug
chemical-spill

## Difficulty
Medium

## Description
Toxic sludge leaked from Tank A (node 1) and is flowing toward the River (node n).

The plant consists of $n$ drains connected by $m$ two-way pipes.
The sludge is attempting to travel from Tank A (node 1) to the River (node $n$).

To prevent this, you can clog specific pipes. Clogging a pipe stops the flow.

Your task is to calculate the **minimum number of pipes** that must be clogged to completely sever all routes between Tank A and the River.

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
We can clog edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of drains and pipes.
- The next $m$ lines describe the pipes. Each line contains two integers $a$ and $b$, indicating a pipe between drain $a$ and drain $b$.

## Output Format
- Return one integer: the minimum number of pipes that need to be clogged.

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
