## Title
Avalanche Prevention

## Slug
avalanche-prevention

## Difficulty
Medium

## Description
Snow is sliding from the Summit (node 1) to the Ski Lodge (node n).

The mountain consists of $n$ plateaus connected by $m$ two-way chutes.
The snow is attempting to travel from the Summit (node 1) to the Lodge (node $n$).

To prevent this, you can barrier specific chutes. Building a barrier in a chute stops the snow.

Your task is to calculate the **minimum number of chutes** that must be blocked to completely sever all routes between the Summit and the Lodge.

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
We can barrier edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of plateaus and chutes.
- The next $m$ lines describe the chutes. Each line contains two integers $a$ and $b$, indicating a chute between plateau $a$ and plateau $b$.

## Output Format
- Return one integer: the minimum number of chutes that need to be blocked.

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
