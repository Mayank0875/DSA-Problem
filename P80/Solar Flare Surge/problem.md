## Title
Solar Flare Surge

## Slug
solar-flare-surge

## Difficulty
Medium

## Description
A flare hits the Satellite (node 1) and surge travels to the Control Room (node n).

The power grid consists of $n$ breakers connected by $m$ two-way cables.
The surge is attempting to travel from the Satellite (node 1) to Control (node $n$).

To prevent this, you can cut specific cables. Cutting a cable isolates the surge.

Your task is to calculate the **minimum number of cables** that must be cut to completely sever all routes between the Satellite and Control.

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
- The first line contains two integers $n$ and $m$: the number of breakers and cables.
- The next $m$ lines describe the cables. Each line contains two integers $a$ and $b$, indicating a cable between breaker $a$ and breaker $b$.

## Output Format
- Return one integer: the minimum number of cables that need to be cut.

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
