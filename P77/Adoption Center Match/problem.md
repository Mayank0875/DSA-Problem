## Title
Adoption Center Match

## Slug
adoption-center-match

## Difficulty
Medium

## Description
An animal shelter tries to match `n` pets with `m` potential adopters.

However, not every pet is compatible with every adopter based on lifestyle compatibility.
You are given a list of `k` compatible pairs, where a specific pet can work with a specific adopter.

Your task is to determine the maximum number of adoptions that can be formed simultaneously. Each pet and each adopter can be assigned to at most one adoption.

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
There are 3 pets and 2 adopters.
Possible valid matching could be:
- pet 1 with adopter 2
- pet 2 with adopter 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only pet 1 and adopter 1 are compatible. The maximum number of operational adoptions is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of pets, adopters, and compatible pairs.
- The pets are numbered `1` to `n` and the adopters are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that pet `a` and adopter `b` are compatible.

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
