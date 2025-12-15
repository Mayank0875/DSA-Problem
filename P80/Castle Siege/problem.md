## Title
Castle Siege

## Slug
castle-siege

## Difficulty
Medium

## Description
Invaders have breached the Outer Gate (node 1) and are running to the Keep (node n).

The castle consists of $n$ courtyards connected by $m$ two-way archways.
The invaders is attempting to travel from the Gate (node 1) to the Keep (node $n$).

To prevent this, you can collapse specific archways. Collapsing an archway blocks the path.

Your task is to calculate the **minimum number of archways** that must be collapsed to completely sever all routes between the Gate and the Keep.

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
- The first line contains two integers $n$ and $m$: the number of courtyards and archways.
- The next $m$ lines describe the archways. Each line contains two integers $a$ and $b$, indicating a archway between courtyard $a$ and courtyard $b$.

## Output Format
- Return one integer: the minimum number of archways that need to be collapsed.

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
