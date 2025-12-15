## Title
Power Plant Grid

## Slug
power-plant-grid

## Difficulty
Medium

## Description
There are `n` generators and `m` substations needing power.

However, not every generator is compatible with every substation due to voltage compatibility.
You are given a list of `k` compatible pairs, where a specific generator can work with a specific substation.

Your task is to determine the maximum number of links that can be formed simultaneously. Each generator and each substation can be assigned to at most one link.

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
There are 3 generators and 2 substations.
Possible valid matching could be:
- generator 1 with substation 2
- generator 2 with substation 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only generator 1 and substation 1 are compatible. The maximum number of operational links is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of generators, substations, and compatible pairs.
- The generators are numbered `1` to `n` and the substations are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that generator `a` and substation `b` are compatible.

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
