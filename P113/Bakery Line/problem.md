## Title
Bakery Line

## Slug
bakery-line

## Difficulty
Medium

## Description
Customers want pastries. The display case has Croissants (0) and Bagels (1) stacked.

There are two types of pastries: **Croissants** (represented by `0`) and **Bagels** (represented by `1`). Each customer has a specific preference and will only accept one type of pastry.

The pastries are prepared in a **stack**, meaning only the top pastry is accessible at any time. The distribution process works as follows:
1. If the customer at the front of the queue prefers the pastry currently on top of the stack, they take it and leave the queue.
2. If they do not like the top pastry, they move to the very back of the queue to wait for another turn.

This cycle continues until either all customers are served, or the customer at the front of the queue (and everyone else behind them) refuses the pastry currently on top of the stack.

Your task is to determine the number of customers who are unable to receive a pastry.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front customer (1) dislikes top pastry (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front customer (1) dislikes top pastry (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front customer (0) takes top pastry (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front customer (0) dislikes top pastry (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all customers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top pastry is `1` (Bagels). Three customers prefer Croissants (`0`) and three prefer Bagels (`1`). After the Bagels customers take their pastries, the stack has `0` (Croissants) on top, but only customers wanting `1` remain. They cycle endlessly. 3 customers remain.

## Input Format
- First line: An integer `n`, the number of customers (and pastries).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of pastries.

## Output Format
- Return a single integer representing the number of customers who cannot get a pastry.

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
