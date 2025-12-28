## Title
Burger Joint

## Slug
burger-joint

## Difficulty
Medium

## Description
Diners order burgers. The chute delivers Cheeseburgers (0) and Hamburgers (1).

There are two types of burgers: **Cheeseburgers** (represented by `0`) and **Hamburgers** (represented by `1`). Each diner has a specific preference and will only accept one type of burger.

The burgers are prepared in a **stack**, meaning only the top burger is accessible at any time. The distribution process works as follows:
1. If the diner at the front of the queue prefers the burger currently on top of the stack, they take it and leave the queue.
2. If they do not like the top burger, they move to the very back of the queue to wait for another turn.

This cycle continues until either all diners are served, or the diner at the front of the queue (and everyone else behind them) refuses the burger currently on top of the stack.

Your task is to determine the number of diners who are unable to receive a burger.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front diner (1) dislikes top burger (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front diner (1) dislikes top burger (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front diner (0) takes top burger (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front diner (0) dislikes top burger (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all diners find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top burger is `1` (Hamburgers). Three diners prefer Cheeseburgers (`0`) and three prefer Hamburgers (`1`). After the Hamburgers diners take their burgers, the stack has `0` (Cheeseburgers) on top, but only diners wanting `1` remain. They cycle endlessly. 3 diners remain.

## Input Format
- First line: An integer `n`, the number of diners (and burgers).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of burgers.

## Output Format
- Return a single integer representing the number of diners who cannot get a burger.

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
