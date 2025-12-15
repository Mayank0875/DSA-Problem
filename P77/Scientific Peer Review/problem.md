## Title
Scientific Peer Review

## Slug
scientific-peer-review

## Difficulty
Medium

## Description
A journal assigns `n` papers to `m` reviewers.

However, not every paper is compatible with every reviewer due to field of study expertise.
You are given a list of `k` compatible pairs, where a specific paper can work with a specific reviewer.

Your task is to determine the maximum number of reviews that can be formed simultaneously. Each paper and each reviewer can be assigned to at most one review.

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
There are 3 papers and 2 reviewers.
Possible valid matching could be:
- paper 1 with reviewer 2
- paper 2 with reviewer 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only paper 1 and reviewer 1 are compatible. The maximum number of operational reviews is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of papers, reviewers, and compatible pairs.
- The papers are numbered `1` to `n` and the reviewers are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that paper `a` and reviewer `b` are compatible.

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
