## Title
Internship Placements

## Slug
internship-placements

## Difficulty
Medium

## Description
A college places `n` interns into `m` startup companies.

However, not every intern is compatible with every startup based on major.
You are given a list of `k` compatible pairs, where a specific intern can work with a specific startup.

Your task is to determine the maximum number of jobs that can be formed simultaneously. Each intern and each startup can be assigned to at most one job.

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
There are 3 interns and 2 startups.
Possible valid matching could be:
- intern 1 with startup 2
- intern 2 with startup 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only intern 1 and startup 1 are compatible. The maximum number of operational jobs is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of interns, startups, and compatible pairs.
- The interns are numbered `1` to `n` and the startups are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that intern `a` and startup `b` are compatible.

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
