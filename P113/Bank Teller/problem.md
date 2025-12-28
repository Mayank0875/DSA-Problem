## Title
Bank Teller

## Slug
bank-teller

## Difficulty
Medium

## Description
Clients want cash. The drawer has $20 (0) and $50 (1) bills.

There are two types of bills: **$20** (represented by `0`) and **$50** (represented by `1`). Each client has a specific preference and will only accept one type of bill.

The bills are prepared in a **stack**, meaning only the top bill is accessible at any time. The distribution process works as follows:
1. If the client at the front of the queue prefers the bill currently on top of the stack, they take it and leave the queue.
2. If they do not like the top bill, they move to the very back of the queue to wait for another turn.

This cycle continues until either all clients are served, or the client at the front of the queue (and everyone else behind them) refuses the bill currently on top of the stack.

Your task is to determine the number of clients who are unable to receive a bill.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front client (1) dislikes top bill (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front client (1) dislikes top bill (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front client (0) takes top bill (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front client (0) dislikes top bill (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all clients find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top bill is `1` ($50). Three clients prefer $20 (`0`) and three prefer $50 (`1`). After the $50 clients take their bills, the stack has `0` ($20) on top, but only clients wanting `1` remain. They cycle endlessly. 3 clients remain.

## Input Format
- First line: An integer `n`, the number of clients (and bills).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of bills.

## Output Format
- Return a single integer representing the number of clients who cannot get a bill.

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
