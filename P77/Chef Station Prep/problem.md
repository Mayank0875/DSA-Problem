## Title
Chef Station Prep

## Slug
chef-station-prep

## Difficulty
Medium

## Description
A head chef assigns `n` cooks to `m` stations.

However, not every cook is compatible with every station based on culinary specialty.
You are given a list of `k` compatible pairs, where a specific cook can work with a specific station.

Your task is to determine the maximum number of assignments that can be formed simultaneously. Each cook and each station can be assigned to at most one assignment.

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
There are 3 cooks and 2 stations.
Possible valid matching could be:
- cook 1 with station 2
- cook 2 with station 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only cook 1 and station 1 are compatible. The maximum number of operational assignments is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of cooks, stations, and compatible pairs.
- The cooks are numbered `1` to `n` and the stations are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that cook `a` and station `b` are compatible.

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
