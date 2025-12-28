## Title
Construction Site

## Slug
construction-site

## Difficulty
Medium

## Description
Workers need bricks. The pallet has Red (0) and Grey (1) bricks stacked.

There are two types of bricks: **Red** (represented by `0`) and **Grey** (represented by `1`). Each worker has a specific preference and will only accept one type of brick.

The bricks are prepared in a **stack**, meaning only the top brick is accessible at any time. The distribution process works as follows:
1. If the worker at the front of the queue prefers the brick currently on top of the stack, they take it and leave the queue.
2. If they do not like the top brick, they move to the very back of the queue to wait for another turn.

This cycle continues until either all workers are served, or the worker at the front of the queue (and everyone else behind them) refuses the brick currently on top of the stack.

Your task is to determine the number of workers who are unable to receive a brick.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front worker (1) dislikes top brick (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front worker (1) dislikes top brick (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front worker (0) takes top brick (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front worker (0) dislikes top brick (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all workers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top brick is `1` (Grey). Three workers prefer Red (`0`) and three prefer Grey (`1`). After the Grey workers take their bricks, the stack has `0` (Red) on top, but only workers wanting `1` remain. They cycle endlessly. 3 workers remain.

## Input Format
- First line: An integer `n`, the number of workers (and bricks).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of bricks.

## Output Format
- Return a single integer representing the number of workers who cannot get a brick.

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
