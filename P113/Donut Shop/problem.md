## Title
Donut Shop

## Slug
donut-shop

## Difficulty
Medium

## Description
Police officers grab donuts. The box has Glazed (0) and Sprinkled (1).

There are two types of donuts: **Glazed** (represented by `0`) and **Sprinkled** (represented by `1`). Each officer has a specific preference and will only accept one type of donut.

The donuts are prepared in a **stack**, meaning only the top donut is accessible at any time. The distribution process works as follows:
1. If the officer at the front of the queue prefers the donut currently on top of the stack, they take it and leave the queue.
2. If they do not like the top donut, they move to the very back of the queue to wait for another turn.

This cycle continues until either all officers are served, or the officer at the front of the queue (and everyone else behind them) refuses the donut currently on top of the stack.

Your task is to determine the number of officers who are unable to receive a donut.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front officer (1) dislikes top donut (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front officer (1) dislikes top donut (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front officer (0) takes top donut (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front officer (0) dislikes top donut (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all officers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top donut is `1` (Sprinkled). Three officers prefer Glazed (`0`) and three prefer Sprinkled (`1`). After the Sprinkled officers take their donuts, the stack has `0` (Glazed) on top, but only officers wanting `1` remain. They cycle endlessly. 3 officers remain.

## Input Format
- First line: An integer `n`, the number of officers (and donuts).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of donuts.

## Output Format
- Return a single integer representing the number of officers who cannot get a donut.

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
