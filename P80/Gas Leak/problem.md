## Title
Gas Leak

## Slug
gas-leak

## Difficulty
Medium

## Description
Gas leaks from the Main Line (node 1) toward the Kitchen (node n).

The piping consists of $n$ valves connected by $m$ two-way tubes.
The gas is attempting to travel from the Main Line (node 1) to the Kitchen (node $n$).

To prevent this, you can crimp specific tubes. Crimping a tube seals the leak.

Your task is to calculate the **minimum number of tubes** that must be crimped to completely sever all routes between the Main Line and the Kitchen.

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
We can crimp edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of valves and tubes.
- The next $m$ lines describe the tubes. Each line contains two integers $a$ and $b$, indicating a tube between valve $a$ and valve $b$.

## Output Format
- Return one integer: the minimum number of tubes that need to be crimped.

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
