## Title
Delivery Drone Routes

## Slug
delivery-drone-routes

## Difficulty
Medium

## Description
A depot has `n` drones and `m` packages ready for delivery.

However, not every drone is compatible with every package due to weight capacity.
You are given a list of `k` compatible pairs, where a specific drone can work with a specific package.

Your task is to determine the maximum number of deliveries that can be formed simultaneously. Each drone and each package can be assigned to at most one delivery.

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
There are 3 drones and 2 packages.
Possible valid matching could be:
- drone 1 with package 2
- drone 2 with package 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only drone 1 and package 1 are compatible. The maximum number of operational deliveries is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of drones, packages, and compatible pairs.
- The drones are numbered `1` to `n` and the packages are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that drone `a` and package `b` are compatible.

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
