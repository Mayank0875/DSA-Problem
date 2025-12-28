## Title
Gym Equipment

## Slug
gym-equipment

## Difficulty
Medium

## Description
Gym members wait for weights. The rack has Dumbbells (0) and Kettlebells (1) stacked.

There are two types of weights: **Dumbbells** (represented by `0`) and **Kettlebells** (represented by `1`). Each member has a specific preference and will only accept one type of weight.

The weights are prepared in a **stack**, meaning only the top weight is accessible at any time. The distribution process works as follows:
1. If the member at the front of the queue prefers the weight currently on top of the stack, they take it and leave the queue.
2. If they do not like the top weight, they move to the very back of the queue to wait for another turn.

This cycle continues until either all members are served, or the member at the front of the queue (and everyone else behind them) refuses the weight currently on top of the stack.

Your task is to determine the number of members who are unable to receive a weight.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front member (1) dislikes top weight (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front member (1) dislikes top weight (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front member (0) takes top weight (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front member (0) dislikes top weight (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all members find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top weight is `1` (Kettlebells). Three members prefer Dumbbells (`0`) and three prefer Kettlebells (`1`). After the Kettlebells members take their weights, the stack has `0` (Dumbbells) on top, but only members wanting `1` remain. They cycle endlessly. 3 members remain.

## Input Format
- First line: An integer `n`, the number of members (and weights).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of weights.

## Output Format
- Return a single integer representing the number of members who cannot get a weight.

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
