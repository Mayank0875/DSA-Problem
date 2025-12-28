## Title
Taxi Stand

## Slug
taxi-stand

## Difficulty
Medium

## Description
Commuters wait for cabs. The line has Sedans (0) and Vans (1).

There are two types of cabs: **Sedans** (represented by `0`) and **Vans** (represented by `1`). Each commuter has a specific preference and will only accept one type of cab.

The cabs are prepared in a **stack**, meaning only the top cab is accessible at any time. The distribution process works as follows:
1. If the commuter at the front of the queue prefers the cab currently on top of the stack, they take it and leave the queue.
2. If they do not like the top cab, they move to the very back of the queue to wait for another turn.

This cycle continues until either all commuters are served, or the commuter at the front of the queue (and everyone else behind them) refuses the cab currently on top of the stack.

Your task is to determine the number of commuters who are unable to receive a cab.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front commuter (1) dislikes top cab (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front commuter (1) dislikes top cab (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front commuter (0) takes top cab (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front commuter (0) dislikes top cab (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all commuters find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top cab is `1` (Vans). Three commuters prefer Sedans (`0`) and three prefer Vans (`1`). After the Vans commuters take their cabs, the stack has `0` (Sedans) on top, but only commuters wanting `1` remain. They cycle endlessly. 3 commuters remain.

## Input Format
- First line: An integer `n`, the number of commuters (and cabs).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of cabs.

## Output Format
- Return a single integer representing the number of commuters who cannot get a cab.

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
