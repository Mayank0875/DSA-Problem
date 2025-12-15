## Title
Garden Planting

## Slug
garden-planting

## Difficulty
Medium

## Description
A landscaper plants `n` saplings in `m` holes.

However, not every sapling is compatible with every hole based on sunlight needs.
You are given a list of `k` compatible pairs, where a specific sapling can work with a specific hole.

Your task is to determine the maximum number of plantings that can be formed simultaneously. Each sapling and each hole can be assigned to at most one planting.

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
There are 3 saplings and 2 holes.
Possible valid matching could be:
- sapling 1 with hole 2
- sapling 2 with hole 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only sapling 1 and hole 1 are compatible. The maximum number of operational plantings is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of saplings, holes, and compatible pairs.
- The saplings are numbered `1` to `n` and the holes are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that sapling `a` and hole `b` are compatible.

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
