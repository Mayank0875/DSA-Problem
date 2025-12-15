## Title
Escaped Convict

## Slug
escaped-convict

## Difficulty
Medium

## Description
A convict escaped Prison (node 1) and runs to the Harbor (node n).

The county consists of $n$ towns connected by $m$ two-way highways.
The convict is attempting to travel from Prison (node 1) to the Harbor (node $n$).

To prevent this, you can blockade specific highways. Blockading a highway stops the car.

Your task is to calculate the **minimum number of highways** that must be blockaded to completely sever all routes between Prison and the Harbor.

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
We can blockade edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of towns and highways.
- The next $m$ lines describe the highways. Each line contains two integers $a$ and $b$, indicating a highway between town $a$ and town $b$.

## Output Format
- Return one integer: the minimum number of highways that need to be blockaded.

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
