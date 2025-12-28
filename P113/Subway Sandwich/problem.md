## Title
Subway Sandwich

## Slug
subway-sandwich

## Difficulty
Medium

## Description
Customers choose bread. The rack holds Italian (0) and Wheat (1).

There are two types of breads: **Italian** (represented by `0`) and **Wheat** (represented by `1`). Each customer has a specific preference and will only accept one type of bread.

The breads are prepared in a **stack**, meaning only the top bread is accessible at any time. The distribution process works as follows:
1. If the customer at the front of the queue prefers the bread currently on top of the stack, they take it and leave the queue.
2. If they do not like the top bread, they move to the very back of the queue to wait for another turn.

This cycle continues until either all customers are served, or the customer at the front of the queue (and everyone else behind them) refuses the bread currently on top of the stack.

Your task is to determine the number of customers who are unable to receive a bread.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front customer (1) dislikes top bread (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front customer (1) dislikes top bread (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front customer (0) takes top bread (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front customer (0) dislikes top bread (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all customers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top bread is `1` (Wheat). Three customers prefer Italian (`0`) and three prefer Wheat (`1`). After the Wheat customers take their breads, the stack has `0` (Italian) on top, but only customers wanting `1` remain. They cycle endlessly. 3 customers remain.

## Input Format
- First line: An integer `n`, the number of customers (and breads).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of breads.

## Output Format
- Return a single integer representing the number of customers who cannot get a bread.

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
