## Title
Postal Mail Route

## Slug
postal-mail-route

## Difficulty
Medium

## Description
A letter is sorted through exactly k distribution centers. Sorting takes time.

You need to find a path from Drop Box (index 1) to Mailbox (index n) that consists of **exactly** `k` sorts.
Each sort connects a source center to a destination center and has a specific time associated with it.

Your goal is to calculate the minimum total time required to travel from Drop Box to Mailbox using exactly `k` sorts. If it is impossible to reach the destination with exactly `k` sorts, return -1.

## Examples

### 1

#### Input
3 4 8
1 2 5
2 3 4
3 1 1
3 2 2

#### Output
27

#### Explanation
We need a path from Drop Box to Mailbox using exactly 8 sorts.
Consider the path: 1 -> 2 -> 3 -> 2 -> 3 -> 2 -> 3 -> 2 -> 3.
Costs: 5 + 4 + 2 + 4 + 2 + 4 + 2 + 4 = 27.
This is the minimum cost possible.

### 2

#### Input
2 1 100
1 2 10

#### Output
-1

#### Explanation
There is only one sort from 1 to 2. It is impossible to make 100 sorts because once you reach node 2, there are no outgoing sorts to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of centers, sorts, and the required number of jumps.
- The next `m` lines describe the sorts. Each line contains three integers `u`, `v`, and `w`: a sort from `u` to `v` with time `w`.

## Output Format
- Return one integer: the minimum total time. If no such path exists, return -1.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ n * (n - 1)
- 1 ≤ k ≤ 10^9
- 1 ≤ u, v ≤ n
- 1 ≤ w ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
