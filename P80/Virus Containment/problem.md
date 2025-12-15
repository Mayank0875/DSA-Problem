## Title
Virus Containment

## Slug
virus-containment

## Difficulty
Medium

## Description
A deadly virus has broken out at the Research Lab (node 1) and is spreading towards the City Center (node n).

The quarantine zone consists of $n$ sectors connected by $m$ two-way transit links.
The virus is attempting to travel from the Lab (node 1) to the City (node $n$).

To prevent this, you can close specific transit links. Closing a link stops the spread in both directions.

Your task is to calculate the **minimum number of transit links** that must be closed to completely sever all routes between the Lab and the City.

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
- The first line contains two integers $n$ and $m$: the number of sectors and transit links.
- The next $m$ lines describe the transit links. Each line contains two integers $a$ and $b$, indicating a transit link between sector $a$ and sector $b$.

## Output Format
- Return one integer: the minimum number of transit links that need to be closed.

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
