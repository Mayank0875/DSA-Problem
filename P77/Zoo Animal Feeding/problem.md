## Title
Zoo Animal Feeding

## Slug
zoo-animal-feeding

## Difficulty
Medium

## Description
Keepers assign `n` special diets to `m` animals.

However, not every diet is compatible with every animal based on species requirement.
You are given a list of `k` compatible pairs, where a specific diet can work with a specific animal.

Your task is to determine the maximum number of feedings that can be formed simultaneously. Each diet and each animal can be assigned to at most one feeding.

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
There are 3 diets and 2 animals.
Possible valid matching could be:
- diet 1 with animal 2
- diet 2 with animal 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only diet 1 and animal 1 are compatible. The maximum number of operational feedings is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of diets, animals, and compatible pairs.
- The diets are numbered `1` to `n` and the animals are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that diet `a` and animal `b` are compatible.

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
