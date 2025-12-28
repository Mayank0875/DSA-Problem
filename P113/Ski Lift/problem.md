## Title
Ski Lift

## Slug
ski-lift

## Difficulty
Medium

## Description
Skiers wait for chairs. The lift has Green (0) and Blue (1) chairs, and skiers are superstitious about color.

There are two types of chairs: **Green** (represented by `0`) and **Blue** (represented by `1`). Each skier has a specific preference and will only accept one type of chair.

The chairs are prepared in a **stack**, meaning only the top chair is accessible at any time. The distribution process works as follows:
1. If the skier at the front of the queue prefers the chair currently on top of the stack, they take it and leave the queue.
2. If they do not like the top chair, they move to the very back of the queue to wait for another turn.

This cycle continues until either all skiers are served, or the skier at the front of the queue (and everyone else behind them) refuses the chair currently on top of the stack.

Your task is to determine the number of skiers who are unable to receive a chair.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front skier (1) dislikes top chair (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front skier (1) dislikes top chair (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front skier (0) takes top chair (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front skier (0) dislikes top chair (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all skiers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top chair is `1` (Blue). Three skiers prefer Green (`0`) and three prefer Blue (`1`). After the Blue skiers take their chairs, the stack has `0` (Green) on top, but only skiers wanting `1` remain. They cycle endlessly. 3 skiers remain.

## Input Format
- First line: An integer `n`, the number of skiers (and chairs).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of chairs.

## Output Format
- Return a single integer representing the number of skiers who cannot get a chair.

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
