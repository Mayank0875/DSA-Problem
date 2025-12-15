## Title
Soccer Transfer Market

## Slug
soccer-transfer-market

## Difficulty
Medium

## Description
Agents match `n` players with `m` clubs looking for signings.

However, not every player is compatible with every club based on position needed.
You are given a list of `k` compatible pairs, where a specific player can work with a specific club.

Your task is to determine the maximum number of transfers that can be formed simultaneously. Each player and each club can be assigned to at most one transfer.

## Examples

### 1

#### Input
3 2 4
1 1
1 2
2 1
3 1

#### Output
2

#### Explanation
There are 3 players and 2 clubs.
Possible valid matching could be:
- player 1 with club 2
- player 2 with club 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only player 1 and club 1 are compatible. The maximum number of operational transfers is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of players, clubs, and compatible pairs.
- The players are numbered `1` to `n` and the clubs are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that player `a` and club `b` are compatible.

## Output Format
- Return one integer: the maximum number of pairs that can be formed.

## Constraints
- 1 ≤ n, m ≤ 500
- 1 ≤ k ≤ 1000
- 1 ≤ a ≤ n
- 1 ≤ b ≤ m

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
