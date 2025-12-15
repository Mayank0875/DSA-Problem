## Title
Water Leak Repair

## Slug
water-leak-repair

## Difficulty
Medium

## Description
A massive leak has occurred at the Main Reservoir (node 1) and water is flowing toward the Electrical Grid (node n).

The pipe network consists of $n$ junctions connected by $m$ two-way pipes.
The water is attempting to travel from the Reservoir (node 1) to the Grid (node $n$).

To prevent this, you can seal specific pipes. Sealing a pipe stops water flow.

Your task is to calculate the **minimum number of pipes** that must be sealed to completely sever all routes between the Reservoir and the Grid.

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
We can seal edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of junctions and pipes.
- The next $m$ lines describe the pipes. Each line contains two integers $a$ and $b$, indicating a pipe between junction $a$ and junction $b$.

## Output Format
- Return one integer: the minimum number of pipes that need to be sealed.

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
