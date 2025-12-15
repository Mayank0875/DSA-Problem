## Title
Server Job Allocation

## Slug
server-job-allocation

## Difficulty
Medium

## Description
A cloud cluster has `n` jobs and `m` servers. Each job needs to be processed by a single server.

However, not every job is compatible with every server due to hardware requirements.
You are given a list of `k` compatible pairs, where a specific job can work with a specific server.

Your task is to determine the maximum number of running jobs that can be formed simultaneously. Each job and each server can be assigned to at most one allocation.

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
There are 3 jobs and 2 servers.
Possible valid matching could be:
- job 1 with server 2
- job 2 with server 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only job 1 and server 1 are compatible. The maximum number of operational running jobs is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of jobs, servers, and compatible pairs.
- The jobs are numbered `1` to `n` and the servers are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that job `a` and server `b` are compatible.

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
