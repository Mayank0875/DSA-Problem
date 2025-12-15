## Title
Diplomatic Message Relay

## Slug
diplomatic-message-relay

## Difficulty
Medium

## Description
A message is relayed through exactly k embassies to ensure secrecy. Each relay takes hours.

You need to find a path from Capital A (index 1) to Capital B (index n) that consists of **exactly** `k` relays.
Each relay connects a source embassy to a destination embassy and has a specific hours associated with it.

Your goal is to calculate the minimum total hours required to travel from Capital A to Capital B using exactly `k` relays. If it is impossible to reach the destination with exactly `k` relays, return -1.

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
We need a path from Capital A to Capital B using exactly 8 relays.
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
There is only one relay from 1 to 2. It is impossible to make 100 relays because once you reach node 2, there are no outgoing relays to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of embassies, relays, and the required number of jumps.
- The next `m` lines describe the relays. Each line contains three integers `u`, `v`, and `w`: a relay from `u` to `v` with hours `w`.

## Output Format
- Return one integer: the minimum total hours. If no such path exists, return -1.

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
