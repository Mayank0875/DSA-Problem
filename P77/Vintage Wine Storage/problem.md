## Title
Vintage Wine Storage

## Slug
vintage-wine-storage

## Difficulty
Medium

## Description
A sommelier places `n` bottles into `m` rack spots.

However, not every bottle is compatible with every spot based on bottle shape.
You are given a list of `k` compatible pairs, where a specific bottle can work with a specific spot.

Your task is to determine the maximum number of storages that can be formed simultaneously. Each bottle and each spot can be assigned to at most one storage.

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
There are 3 bottles and 2 spots.
Possible valid matching could be:
- bottle 1 with spot 2
- bottle 2 with spot 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only bottle 1 and spot 1 are compatible. The maximum number of operational storages is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of bottles, spots, and compatible pairs.
- The bottles are numbered `1` to `n` and the spots are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that bottle `a` and spot `b` are compatible.

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
