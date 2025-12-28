## Title
Shoe Store

## Slug
shoe-store

## Difficulty
Medium

## Description
Runners try on shoes. The clerk brings Left (0) and Right (1) shoes from a messy pile.

There are two types of shoes: **Left** (represented by `0`) and **Right** (represented by `1`). Each runner has a specific preference and will only accept one type of shoe.

The shoes are prepared in a **stack**, meaning only the top shoe is accessible at any time. The distribution process works as follows:
1. If the runner at the front of the queue prefers the shoe currently on top of the stack, they take it and leave the queue.
2. If they do not like the top shoe, they move to the very back of the queue to wait for another turn.

This cycle continues until either all runners are served, or the runner at the front of the queue (and everyone else behind them) refuses the shoe currently on top of the stack.

Your task is to determine the number of runners who are unable to receive a shoe.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front runner (1) dislikes top shoe (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front runner (1) dislikes top shoe (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front runner (0) takes top shoe (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front runner (0) dislikes top shoe (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all runners find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top shoe is `1` (Right). Three runners prefer Left (`0`) and three prefer Right (`1`). After the Right runners take their shoes, the stack has `0` (Left) on top, but only runners wanting `1` remain. They cycle endlessly. 3 runners remain.

## Input Format
- First line: An integer `n`, the number of runners (and shoes).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of shoes.

## Output Format
- Return a single integer representing the number of runners who cannot get a shoe.

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
