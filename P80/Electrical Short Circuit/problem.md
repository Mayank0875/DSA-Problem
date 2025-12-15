## Title
Electrical Short Circuit

## Slug
electrical-short-circuit

## Difficulty
Medium

## Description
A dangerous current surge begins at the Transformer (node 1) and heads for the Mainframe (node n).

The circuit board consists of $n$ components connected by $m$ two-way wires.
The surge is attempting to travel from the Transformer (node 1) to the Mainframe (node $n$).

To prevent this, you can cut specific wires. Cutting a wire stops the current.

Your task is to calculate the **minimum number of wires** that must be cut to completely sever all routes between the Transformer and the Mainframe.

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
We can cut edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of components and wires.
- The next $m$ lines describe the wires. Each line contains two integers $a$ and $b$, indicating a wire between component $a$ and component $b$.

## Output Format
- Return one integer: the minimum number of wires that need to be cut.

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
