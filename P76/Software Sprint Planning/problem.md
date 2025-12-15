## Title
Software Sprint Planning

## Slug
software-sprint-planning

## Difficulty
Hard

## Description
A project manager divides `n` tasks into `k` development sprints. Tasks have story points and must be done in order. The 'burnout risk' for a sprint is the square of the total story points assigned to it.

You must partition the sequence of tasks into exactly `k` non-empty contiguous sprints.
Each sprint corresponds to a sprint.
The "burnout risk" for a sprint is calculated as the **square of the sum** of the story points of the tasks in that sprint.

Your goal is to minimize the total burnout risk (the sum of the burnout risk values of all `k` sprints).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the tasks into 3 sprints: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total burnout risk is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 sprint is allowed, containing all tasks. Sum = 15. burnout risk = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of tasks and the required number of sprints.
- The second line contains `n` integers representing the story points of each task.

## Output Format
- Return one integer: the minimum total burnout risk.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
