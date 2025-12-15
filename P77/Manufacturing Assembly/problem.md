## Title
Manufacturing Assembly

## Slug
manufacturing-assembly

## Difficulty
Medium

## Description
A factory matches `n` parts with `m` chassis on the line.

However, not every part is compatible with every chassis due to model specifications.
You are given a list of `k` compatible pairs, where a specific part can work with a specific chassis.

Your task is to determine the maximum number of assemblies that can be formed simultaneously. Each part and each chassis can be assigned to at most one assembly.

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
There are 3 parts and 2 chassis.
Possible valid matching could be:
- part 1 with chassis 2
- part 2 with chassis 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only part 1 and chassis 1 are compatible. The maximum number of operational assemblies is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of parts, chassis, and compatible pairs.
- The parts are numbered `1` to `n` and the chassis are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that part `a` and chassis `b` are compatible.

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
