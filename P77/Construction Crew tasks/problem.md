## Title
Construction Crew tasks

## Slug
construction-crew-tasks

## Difficulty
Medium

## Description
A foreman assigns `n` workers to `m` heavy machines.

However, not every worker is compatible with every machine due to license class.
You are given a list of `k` compatible pairs, where a specific worker can work with a specific machine.

Your task is to determine the maximum number of operators that can be formed simultaneously. Each worker and each machine can be assigned to at most one operation.

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
There are 3 workers and 2 machines.
Possible valid matching could be:
- worker 1 with machine 2
- worker 2 with machine 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only worker 1 and machine 1 are compatible. The maximum number of operational operators is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of workers, machines, and compatible pairs.
- The workers are numbered `1` to `n` and the machines are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that worker `a` and machine `b` are compatible.

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
