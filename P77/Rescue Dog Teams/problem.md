## Title
Rescue Dog Teams

## Slug
rescue-dog-teams

## Difficulty
Medium

## Description
A unit pairs `n` handlers with `m` rescue dogs.

However, not every handler is compatible with every dog based on training specialization.
You are given a list of `k` compatible pairs, where a specific handler can work with a specific dog.

Your task is to determine the maximum number of teams that can be formed simultaneously. Each handler and each dog can be assigned to at most one team.

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
There are 3 handlers and 2 dogs.
Possible valid matching could be:
- handler 1 with dog 2
- handler 2 with dog 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only handler 1 and dog 1 are compatible. The maximum number of operational teams is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of handlers, dogs, and compatible pairs.
- The handlers are numbered `1` to `n` and the dogs are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that handler `a` and dog `b` are compatible.

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
