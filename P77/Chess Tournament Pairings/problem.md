## Title
Chess Tournament Pairings

## Slug
chess-tournament-pairings

## Difficulty
Medium

## Description
Arbiters pair `n` white-piece players against `m` black-piece players.

However, not every white player is compatible with every black player based on ELO rating range.
You are given a list of `k` compatible pairs, where a specific white player can work with a specific black player.

Your task is to determine the maximum number of games that can be formed simultaneously. Each white player and each black player can be assigned to at most one game.

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
There are 3 white players and 2 black players.
Possible valid matching could be:
- white player 1 with black player 2
- white player 2 with black player 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only white player 1 and black player 1 are compatible. The maximum number of operational games is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of white players, black players, and compatible pairs.
- The white players are numbered `1` to `n` and the black players are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that white player `a` and black player `b` are compatible.

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
