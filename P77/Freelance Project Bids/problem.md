## Title
Freelance Project Bids

## Slug
freelance-project-bids

## Difficulty
Medium

## Description
There are `n` freelancers and `m` projects. Freelancers bid on projects they can complete.

However, not every freelancer is compatible with every project due to skill set matches.
You are given a list of `k` compatible pairs, where a specific freelancer can work with a specific project.

Your task is to determine the maximum number of contracts that can be formed simultaneously. Each freelancer and each project can be assigned to at most one contract.

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
There are 3 freelancers and 2 projects.
Possible valid matching could be:
- freelancer 1 with project 2
- freelancer 2 with project 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only freelancer 1 and project 1 are compatible. The maximum number of operational contracts is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of freelancers, projects, and compatible pairs.
- The freelancers are numbered `1` to `n` and the projects are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that freelancer `a` and project `b` are compatible.

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
