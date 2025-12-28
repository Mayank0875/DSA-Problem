## Title
Car Wash

## Slug
car-wash

## Difficulty
Medium

## Description
Cars line up for a wash. The automated bay offers Wax (0) or Polish (1) cycles.

There are two types of cycles: **Wax** (represented by `0`) and **Polish** (represented by `1`). Each car has a specific preference and will only accept one type of cycle.

The cycles are prepared in a **stack**, meaning only the top cycle is accessible at any time. The distribution process works as follows:
1. If the car at the front of the queue prefers the cycle currently on top of the stack, they take it and leave the queue.
2. If they do not like the top cycle, they move to the very back of the queue to wait for another turn.

This cycle continues until either all cars are served, or the car at the front of the queue (and everyone else behind them) refuses the cycle currently on top of the stack.

Your task is to determine the number of cars who are unable to receive a cycle.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front car (1) dislikes top cycle (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front car (1) dislikes top cycle (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front car (0) takes top cycle (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front car (0) dislikes top cycle (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all cars find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top cycle is `1` (Polish). Three cars prefer Wax (`0`) and three prefer Polish (`1`). After the Polish cars take their cycles, the stack has `0` (Wax) on top, but only cars wanting `1` remain. They cycle endlessly. 3 cars remain.

## Input Format
- First line: An integer `n`, the number of cars (and cycles).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of cycles.

## Output Format
- Return a single integer representing the number of cars who cannot get a cycle.

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
