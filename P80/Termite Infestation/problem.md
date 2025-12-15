## Title
Termite Infestation

## Slug
termite-infestation

## Difficulty
Medium

## Description
Termites eat from the Foundation (node 1) up to the Roof (node n).

The woodframe consists of $n$ beams connected by $m$ two-way studs.
The termites is attempting to travel from the Foundation (node 1) to the Roof (node $n$).

To prevent this, you can treat specific studs. Chemically treating a stud stops them.

Your task is to calculate the **minimum number of studs** that must be treated to completely sever all routes between the Foundation and the Roof.

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
We can treat edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of beams and studs.
- The next $m$ lines describe the studs. Each line contains two integers $a$ and $b$, indicating a stud between beam $a$ and beam $b$.

## Output Format
- Return one integer: the minimum number of studs that need to be treated.

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
