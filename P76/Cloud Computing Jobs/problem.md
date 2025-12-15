## Title
Cloud Computing Jobs

## Slug
cloud-computing-jobs

## Difficulty
Hard

## Description
A scheduler receives `n` jobs. It assigns them to `k` virtual machines (VMs). Jobs are processed sequentially. The 'thermal throttling' risk of a VM is the square of the total CPU cycles of its jobs.

You must partition the sequence of jobs into exactly `k` non-empty contiguous assignments.
Each assignment corresponds to a VM.
The "throttling risk" for a VM is calculated as the **square of the sum** of the CPU cycles of the jobs in that assignment.

Your goal is to minimize the total throttling risk (the sum of the throttling risk values of all `k` assignments).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the jobs into 3 assignments: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total throttling risk is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 assignment is allowed, containing all jobs. Sum = 15. throttling risk = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of jobs and the required number of assignments.
- The second line contains `n` integers representing the CPU cycles of each job.

## Output Format
- Return one integer: the minimum total throttling risk.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
