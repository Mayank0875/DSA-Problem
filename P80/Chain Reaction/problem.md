## Title
Chain Reaction

## Slug
chain-reaction

## Difficulty
Medium

## Description
A reaction starts at the Core (node 1) and spreads to the Shell (node n).

The reactor consists of $n$ cells connected by $m$ two-way links.
The reaction is attempting to travel from the Core (node 1) to the Shell (node $n$).

To prevent this, you can sever specific links. Severing a link stops the reaction.

Your task is to calculate the **minimum number of links** that must be severed to completely sever all routes between the Core and the Shell.

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
We can sever edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of cells and links.
- The next $m$ lines describe the links. Each line contains two integers $a$ and $b$, indicating a link between cell $a$ and cell $b$.

## Output Format
- Return one integer: the minimum number of links that need to be severed.

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
