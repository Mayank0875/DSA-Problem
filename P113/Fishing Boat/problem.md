## Title
Fishing Boat

## Slug
fishing-boat

## Difficulty
Medium

## Description
Fishermen sort catch. The net holds Tuna (0) and Salmon (1).

There are two types of fish: **Tuna** (represented by `0`) and **Salmon** (represented by `1`). Each fisherman has a specific preference and will only accept one type of fish.

The fish are prepared in a **stack**, meaning only the top fish is accessible at any time. The distribution process works as follows:
1. If the fisherman at the front of the queue prefers the fish currently on top of the stack, they take it and leave the queue.
2. If they do not like the top fish, they move to the very back of the queue to wait for another turn.

This cycle continues until either all fishermen are served, or the fisherman at the front of the queue (and everyone else behind them) refuses the fish currently on top of the stack.

Your task is to determine the number of fishermen who are unable to receive a fish.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front fisherman (1) dislikes top fish (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front fisherman (1) dislikes top fish (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front fisherman (0) takes top fish (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front fisherman (0) dislikes top fish (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all fishermen find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top fish is `1` (Salmon). Three fishermen prefer Tuna (`0`) and three prefer Salmon (`1`). After the Salmon fishermen take their fish, the stack has `0` (Tuna) on top, but only fishermen wanting `1` remain. They cycle endlessly. 3 fishermen remain.

## Input Format
- First line: An integer `n`, the number of fishermen (and fish).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of fish.

## Output Format
- Return a single integer representing the number of fishermen who cannot get a fish.

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
