## Title
Gas Station

## Slug
gas-station

## Difficulty
Medium

## Description
Cars wait for pumps. The station has Regular (0) and Premium (1) nozzles.

There are two types of nozzles: **Regular** (represented by `0`) and **Premium** (represented by `1`). Each driver has a specific preference and will only accept one type of nozzle.

The nozzles are prepared in a **stack**, meaning only the top nozzle is accessible at any time. The distribution process works as follows:
1. If the driver at the front of the queue prefers the nozzle currently on top of the stack, they take it and leave the queue.
2. If they do not like the top nozzle, they move to the very back of the queue to wait for another turn.

This cycle continues until either all drivers are served, or the driver at the front of the queue (and everyone else behind them) refuses the nozzle currently on top of the stack.

Your task is to determine the number of drivers who are unable to receive a nozzle.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front driver (1) dislikes top nozzle (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front driver (1) dislikes top nozzle (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front driver (0) takes top nozzle (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front driver (0) dislikes top nozzle (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all drivers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top nozzle is `1` (Premium). Three drivers prefer Regular (`0`) and three prefer Premium (`1`). After the Premium drivers take their nozzles, the stack has `0` (Regular) on top, but only drivers wanting `1` remain. They cycle endlessly. 3 drivers remain.

## Input Format
- First line: An integer `n`, the number of drivers (and nozzles).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of nozzles.

## Output Format
- Return a single integer representing the number of drivers who cannot get a nozzle.

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
