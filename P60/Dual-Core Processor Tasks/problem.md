## Title
Dual-Core Processor Tasks

## Slug
dual-core-processor-tasks

## Difficulty
Easy

## Description
A scheduler assigns tasks to a CPU. Even-numbered slots are reserved for background processes and must be sorted by priority in ascending order. Odd-numbered slots are for high-performance tasks and must be sorted by priority in descending order. Given the priority values of the tasks, determine the schedule.

## Examples

### 1

#### Input
4
4 1 2 3

#### Output
2 3 4 1

#### Explanation
Values at even indices (0, 2): [4, 2]. Sorted ascending: [2, 4].
Values at odd indices (1, 3): [1, 3]. Sorted descending: [3, 1].
Merged result: Index 0->2, Index 1->3, Index 2->4, Index 3->1. Result: [2, 3, 4, 1].

### 2

#### Input
2
2 1

#### Output
2 1

#### Explanation
Even index 0: [2] -> Sorted: [2].
Odd index 1: [1] -> Sorted: [1].
Result: [2, 1].

## Input Format
- The first line contains an integer n, the number of elements.
- The second line contains n space-separated integers representing the array.

## Output Format
- Return an array containing the n integers in their modified order.

## Constraints
- 1 ≤ n ≤ 10^4
- -10^9 ≤ values[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting
