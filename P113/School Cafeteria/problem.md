## Title
School Cafeteria

## Slug
school-cafeteria

## Difficulty
Medium

## Description
Students are lining up for lunch. The cafeteria offers two types of sandwiches: Circular (0) and Square (1).

There are two types of sandwiches: **Circular Sandwiches** (represented by `0`) and **Square Sandwiches** (represented by `1`). Each student has a specific preference and will only accept one type of sandwich.

The sandwiches are prepared in a **stack**, meaning only the top sandwich is accessible at any time. The distribution process works as follows:
1. If the student at the front of the queue prefers the sandwich currently on top of the stack, they take it and leave the queue.
2. If they do not like the top sandwich, they move to the very back of the queue to wait for another turn.

This cycle continues until either all students are served, or the student at the front of the queue (and everyone else behind them) refuses the sandwich currently on top of the stack.

Your task is to determine the number of students who are unable to receive a sandwich.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front student (1) dislikes top sandwich (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front student (1) dislikes top sandwich (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front student (0) takes top sandwich (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front student (0) dislikes top sandwich (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all students find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top sandwich is `1` (Square Sandwiches). Three students prefer Circular Sandwiches (`0`) and three prefer Square Sandwiches (`1`). After the Square Sandwiches students take their sandwiches, the stack has `0` (Circular Sandwiches) on top, but only students wanting `1` remain. They cycle endlessly. 3 students remain.

## Input Format
- First line: An integer `n`, the number of students (and sandwiches).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of sandwiches.

## Output Format
- Return a single integer representing the number of students who cannot get a sandwich.

## Constraints
- 1 ≤ n ≤ 100
- `preferences[i]` is `0` or `1`.
- `stack[i]` is `0` or `1`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, queue, array
