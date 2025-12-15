## Title
Contraband Flow

## Slug
contraband-flow

## Difficulty
Medium

## Description
Items move from the Drop Zone (node 1) to the Safe House (node n).

The underground consists of $n$ cellars connected by $m$ two-way passages.
The contraband is attempting to travel from the Drop Zone (node 1) to the Safe House (node $n$).

To prevent this, you can collapse specific passages. Collapsing a passage stops the flow.

Your task is to calculate the **minimum number of passages** that must be collapsed to completely sever all routes between the Drop Zone and the Safe House.

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
We can collapse edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of cellars and passages.
- The next $m$ lines describe the passages. Each line contains two integers $a$ and $b$, indicating a passage between cellar $a$ and cellar $b$.

## Output Format
- Return one integer: the minimum number of passages that need to be collapsed.

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
