## Title
Job Fair Interviews

## Slug
job-fair-interviews

## Difficulty
Medium

## Description
A job fair has `n` candidates and `m` companies. Candidates want interviews with companies they are interested in.

However, not every candidate is compatible with every company based on skill matching.
You are given a list of `k` compatible pairs, where a specific candidate can work with a specific company.

Your task is to determine the maximum number of interviews that can be formed simultaneously. Each candidate and each company can be assigned to at most one interview.

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
There are 3 candidates and 2 companies.
Possible valid matching could be:
- candidate 1 with company 2
- candidate 2 with company 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only candidate 1 and company 1 are compatible. The maximum number of operational interviews is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of candidates, companies, and compatible pairs.
- The candidates are numbered `1` to `n` and the companies are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that candidate `a` and company `b` are compatible.

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
