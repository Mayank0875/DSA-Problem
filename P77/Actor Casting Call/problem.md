## Title
Actor Casting Call

## Slug
actor-casting-call

## Difficulty
Medium

## Description
A studio casts `n` actors for `m` roles in a new movie.

However, not every actor is compatible with every role based on audition fit.
You are given a list of `k` compatible pairs, where a specific actor can work with a specific role.

Your task is to determine the maximum number of castings that can be formed simultaneously. Each actor and each role can be assigned to at most one casting.

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
There are 3 actors and 2 roles.
Possible valid matching could be:
- actor 1 with role 2
- actor 2 with role 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only actor 1 and role 1 are compatible. The maximum number of operational castings is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of actors, roles, and compatible pairs.
- The actors are numbered `1` to `n` and the roles are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that actor `a` and role `b` are compatible.

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
