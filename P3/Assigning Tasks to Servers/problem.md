## Title

Assigning Tasks to Servers

## Slug

assigning-tasks-servers

## Difficulty

Easy

## Description

You manage a cluster of servers. Each server can handle one or two tasks simultaneously. However, the combined 'computational load' (represented numerically) of tasks assigned to a single server cannot exceed a maximum limit `x`. You have `n` tasks, each with a specific computational load. Determine the minimum number of servers needed to run all tasks, ensuring no server's load limit is violated.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One minimal server assignment:
    - Server 1: Task with load 2 and task with load 7 (Total load 9 <= 10)
    - Server 2: Task with load 3 (Total load 3 <= 10)
    - Server 3: Task with load 9 (Total load 9 <= 10)
This requires 3 servers.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One minimal server assignment:
    - Server 1: Task with load 2 and task with load 3 (Total load 5 <= 5)
    - Server 2: Two tasks with load 2 (Total load 4 <= 5)
    - Server 3: Task with load 4 (Total load 4 <= 5)
This requires 3 servers.

## Input Format

- The first line contains two integers n and x: the number of tasks and the maximum computational load per server.
- The second line contains n integers p_1, p_2, ..., p_n: the computational load of each task.

## Output Format

- Return a single integer: the minimum number of servers required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers