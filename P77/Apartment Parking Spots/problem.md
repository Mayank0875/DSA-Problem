## Title
Apartment Parking Spots

## Slug
apartment-parking-spots

## Difficulty
Medium

## Description
A building has `n` tenants requesting `m` parking spots.

However, not every tenant is compatible with every spot based on vehicle size.
You are given a list of `k` compatible pairs, where a specific tenant can work with a specific spot.

Your task is to determine the maximum number of assignments that can be formed simultaneously. Each tenant and each spot can be assigned to at most one assignment.

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
There are 3 tenants and 2 spots.
Possible valid matching could be:
- tenant 1 with spot 2
- tenant 2 with spot 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only tenant 1 and spot 1 are compatible. The maximum number of operational assignments is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of tenants, spots, and compatible pairs.
- The tenants are numbered `1` to `n` and the spots are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that tenant `a` and spot `b` are compatible.

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
