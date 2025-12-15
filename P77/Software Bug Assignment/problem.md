## Title
Software Bug Assignment

## Slug
software-bug-assignment

## Difficulty
Medium

## Description
A tech lead assigns `n` bugs to `m` developers. Each bug fixes one issue.

However, not every bug is compatible with every developer due to programming language expertise.
You are given a list of `k` compatible pairs, where a specific bug can work with a specific developer.

Your task is to determine the maximum number of fixed bugs that can be formed simultaneously. Each bug and each developer can be assigned to at most one fix.

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
There are 3 bugs and 2 developers.
Possible valid matching could be:
- bug 1 with developer 2
- bug 2 with developer 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only bug 1 and developer 1 are compatible. The maximum number of operational fixed bugs is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of bugs, developers, and compatible pairs.
- The bugs are numbered `1` to `n` and the developers are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that bug `a` and developer `b` are compatible.

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
