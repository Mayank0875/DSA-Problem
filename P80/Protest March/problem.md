## Title
Protest March

## Slug
protest-march

## Difficulty
Medium

## Description
Protesters march from the Park (node 1) to the Capitol (node n).

The streets consists of $n$ squares connected by $m$ two-way avenues.
The march is attempting to travel from the Park (node 1) to the Capitol (node $n$).

To prevent this, you can block specific avenues. Blocking an avenue redirects them.

Your task is to calculate the **minimum number of avenues** that must be blocked to completely sever all routes between the Park and the Capitol.

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
We can block edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of squares and avenues.
- The next $m$ lines describe the avenues. Each line contains two integers $a$ and $b$, indicating a avenue between square $a$ and square $b$.

## Output Format
- Return one integer: the minimum number of avenues that need to be blocked.

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
