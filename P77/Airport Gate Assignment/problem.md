## Title
Airport Gate Assignment

## Slug
airport-gate-assignment

## Difficulty
Medium

## Description
Traffic control assigns `n` incoming planes to `m` gates.

However, not every plane is compatible with every gate based on aircraft size.
You are given a list of `k` compatible pairs, where a specific plane can work with a specific gate.

Your task is to determine the maximum number of dockings that can be formed simultaneously. Each plane and each gate can be assigned to at most one docking.

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
There are 3 planes and 2 gates.
Possible valid matching could be:
- plane 1 with gate 2
- plane 2 with gate 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only plane 1 and gate 1 are compatible. The maximum number of operational dockings is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of planes, gates, and compatible pairs.
- The planes are numbered `1` to `n` and the gates are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that plane `a` and gate `b` are compatible.

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
