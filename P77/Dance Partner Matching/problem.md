## Title
Dance Partner Matching

## Slug
dance-partner-matching

## Difficulty
Medium

## Description
A dance school has `n` leaders and `m` followers for a tango class. They need to pair up for the practice session.

However, not every leader is compatible with every follower based on height preferences.
You are given a list of `k` compatible pairs, where a specific leader can work with a specific follower.

Your task is to determine the maximum number of couples that can be formed simultaneously. Each leader and each follower can be assigned to at most one couple.

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
There are 3 leaders and 2 followers.
Possible valid matching could be:
- leader 1 with follower 2
- leader 2 with follower 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only leader 1 and follower 1 are compatible. The maximum number of operational couples is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of leaders, followers, and compatible pairs.
- The leaders are numbered `1` to `n` and the followers are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that leader `a` and follower `b` are compatible.

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
