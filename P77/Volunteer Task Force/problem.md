## Title
Volunteer Task Force

## Slug
volunteer-task-force

## Difficulty
Medium

## Description
A charity assigns `n` volunteers to `m` community tasks.

However, not every volunteer is compatible with every task due to physical ability.
You are given a list of `k` compatible pairs, where a specific volunteer can work with a specific task.

Your task is to determine the maximum number of assignments that can be formed simultaneously. Each volunteer and each task can be assigned to at most one assignment.

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
There are 3 volunteers and 2 tasks.
Possible valid matching could be:
- volunteer 1 with task 2
- volunteer 2 with task 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only volunteer 1 and task 1 are compatible. The maximum number of operational assignments is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of volunteers, tasks, and compatible pairs.
- The volunteers are numbered `1` to `n` and the tasks are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that volunteer `a` and task `b` are compatible.

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
