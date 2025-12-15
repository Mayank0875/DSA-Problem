## Title
Tennis Tournament Seeds

## Slug
tennis-tournament-seeds

## Difficulty
Medium

## Description
The organizer pairs `n` players from Team A against `m` players from Team B.

However, not every player A is compatible with every player B based on rank compatibility.
You are given a list of `k` compatible pairs, where a specific player A can work with a specific player B.

Your task is to determine the maximum number of matches that can be formed simultaneously. Each player A and each player B can be assigned to at most one match.

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
There are 3 players A and 2 players B.
Possible valid matching could be:
- player A 1 with player B 2
- player A 2 with player B 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only player A 1 and player B 1 are compatible. The maximum number of operational matches is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of players A, players B, and compatible pairs.
- The players A are numbered `1` to `n` and the players B are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that player A `a` and player B `b` are compatible.

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
