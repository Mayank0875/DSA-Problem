## Title
Fashion Show Outfits

## Slug
fashion-show-outfits

## Difficulty
Medium

## Description
A designer fits `n` models with `m` outfits.

However, not every model is compatible with every outfit based on size measurements.
You are given a list of `k` compatible pairs, where a specific model can work with a specific outfit.

Your task is to determine the maximum number of looks that can be formed simultaneously. Each model and each outfit can be assigned to at most one look.

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
There are 3 models and 2 outfits.
Possible valid matching could be:
- model 1 with outfit 2
- model 2 with outfit 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only model 1 and outfit 1 are compatible. The maximum number of operational looks is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of models, outfits, and compatible pairs.
- The models are numbered `1` to `n` and the outfits are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that model `a` and outfit `b` are compatible.

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
