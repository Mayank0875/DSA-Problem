## Title
Military Supply Line

## Slug
military-supply-line

## Difficulty
Medium

## Description
Enemy forces are moving supplies from their Base (node 1) to the Front Line (node n).

The logistics map consists of $n$ outposts connected by $m$ two-way roads.
The supply convoy is attempting to travel from the Base (node 1) to the Front (node $n$).

To prevent this, you can bomb specific roads. Bombing a road cuts off transport.

Your task is to calculate the **minimum number of roads** that must be bombed to completely sever all routes between the Base and the Front.

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
We can bomb edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of outposts and roads.
- The next $m$ lines describe the roads. Each line contains two integers $a$ and $b$, indicating a road between outpost $a$ and outpost $b$.

## Output Format
- Return one integer: the minimum number of roads that need to be bombed.

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
