## Title
Flower Shop

## Slug
flower-shop

## Difficulty
Medium

## Description
Florists need stems. The bucket holds Roses (0) and Tulips (1).

There are two types of flowers: **Roses** (represented by `0`) and **Tulips** (represented by `1`). Each florist has a specific preference and will only accept one type of flower.

The flowers are prepared in a **stack**, meaning only the top flower is accessible at any time. The distribution process works as follows:
1. If the florist at the front of the queue prefers the flower currently on top of the stack, they take it and leave the queue.
2. If they do not like the top flower, they move to the very back of the queue to wait for another turn.

This cycle continues until either all florists are served, or the florist at the front of the queue (and everyone else behind them) refuses the flower currently on top of the stack.

Your task is to determine the number of florists who are unable to receive a flower.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front florist (1) dislikes top flower (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front florist (1) dislikes top flower (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front florist (0) takes top flower (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front florist (0) dislikes top flower (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all florists find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top flower is `1` (Tulips). Three florists prefer Roses (`0`) and three prefer Tulips (`1`). After the Tulips florists take their flowers, the stack has `0` (Roses) on top, but only florists wanting `1` remain. They cycle endlessly. 3 florists remain.

## Input Format
- First line: An integer `n`, the number of florists (and flowers).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of flowers.

## Output Format
- Return a single integer representing the number of florists who cannot get a flower.

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
