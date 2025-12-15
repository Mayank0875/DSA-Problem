## Title
Music Festival Lineup

## Slug
music-festival-lineup

## Difficulty
Medium

## Description
Promoters assign `n` bands to `m` time slots.

However, not every band is compatible with every slot based on popularity tier.
You are given a list of `k` compatible pairs, where a specific band can work with a specific slot.

Your task is to determine the maximum number of performances that can be formed simultaneously. Each band and each slot can be assigned to at most one performance.

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
There are 3 bands and 2 slots.
Possible valid matching could be:
- band 1 with slot 2
- band 2 with slot 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only band 1 and slot 1 are compatible. The maximum number of operational performances is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of bands, slots, and compatible pairs.
- The bands are numbered `1` to `n` and the slots are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that band `a` and slot `b` are compatible.

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
