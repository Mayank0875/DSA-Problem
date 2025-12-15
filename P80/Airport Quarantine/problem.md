## Title
Airport Quarantine

## Slug
airport-quarantine

## Difficulty
Medium

## Description
An infected passenger arrived at Gate 1 and is walking to the Taxi Stand (node n).

The airport consists of $n$ terminals connected by $m$ two-way walkways.
The passenger is attempting to travel from Gate 1 (node 1) to the Taxi Stand (node $n$).

To prevent this, you can close specific walkways. Closing a walkway contains the passenger.

Your task is to calculate the **minimum number of walkways** that must be closed to completely sever all routes between Gate 1 and the Taxi Stand.

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
We can close edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of terminals and walkways.
- The next $m$ lines describe the walkways. Each line contains two integers $a$ and $b$, indicating a walkway between terminal $a$ and terminal $b$.

## Output Format
- Return one integer: the minimum number of walkways that need to be closed.

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
