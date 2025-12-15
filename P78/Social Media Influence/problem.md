## Title
Social Media Influence

## Slug
social-media-influence

## Difficulty
Medium

## Description
A viral post is shared exactly k times. Each share moves from user to user and takes time to propagate.

You need to find a path from Original Poster (index 1) to Target Influencer (index n) that consists of **exactly** `k` shares.
Each share connects a source user to a destination user and has a specific propagation time associated with it.

Your goal is to calculate the minimum total propagation time required to travel from Original Poster to Target Influencer using exactly `k` shares. If it is impossible to reach the destination with exactly `k` shares, return -1.

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
We need a path from Original Poster to Target Influencer using exactly 8 shares.
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
There is only one share from 1 to 2. It is impossible to make 100 shares because once you reach node 2, there are no outgoing shares to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of users, shares, and the required number of jumps.
- The next `m` lines describe the shares. Each line contains three integers `u`, `v`, and `w`: a share from `u` to `v` with propagation time `w`.

## Output Format
- Return one integer: the minimum total propagation time. If no such path exists, return -1.

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
