## Title
Warehouse Docking

## Slug
warehouse-docking

## Difficulty
Medium

## Description
A logistics hub has `n` trucks and `m` loading docks. Trucks need to unload cargo.

However, not every truck is compatible with every dock due to vehicle size limits.
You are given a list of `k` compatible pairs, where a specific truck can work with a specific dock.

Your task is to determine the maximum number of unloading ops that can be formed simultaneously. Each truck and each dock can be assigned to at most one operation.

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
There are 3 trucks and 2 docks.
Possible valid matching could be:
- truck 1 with dock 2
- truck 2 with dock 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only truck 1 and dock 1 are compatible. The maximum number of operational unloading ops is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of trucks, docks, and compatible pairs.
- The trucks are numbered `1` to `n` and the docks are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that truck `a` and dock `b` are compatible.

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
