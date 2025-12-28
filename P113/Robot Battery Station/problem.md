## Title
Robot Battery Station

## Slug
robot-battery-station

## Difficulty
Medium

## Description
Robots queue to swap batteries. The station dispenses Lithium (0) and Nuclear (1) cells from a vertical dispenser.

There are two types of batteries: **Lithium Cells** (represented by `0`) and **Nuclear Cells** (represented by `1`). Each robot has a specific preference and will only accept one type of battery.

The batteries are prepared in a **stack**, meaning only the top battery is accessible at any time. The distribution process works as follows:
1. If the robot at the front of the queue prefers the battery currently on top of the stack, they take it and leave the queue.
2. If they do not like the top battery, they move to the very back of the queue to wait for another turn.

This cycle continues until either all robots are served, or the robot at the front of the queue (and everyone else behind them) refuses the battery currently on top of the stack.

Your task is to determine the number of robots who are unable to receive a battery.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front robot (1) dislikes top battery (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front robot (1) dislikes top battery (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front robot (0) takes top battery (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front robot (0) dislikes top battery (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all robots find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top battery is `1` (Nuclear Cells). Three robots prefer Lithium Cells (`0`) and three prefer Nuclear Cells (`1`). After the Nuclear Cells robots take their batteries, the stack has `0` (Lithium Cells) on top, but only robots wanting `1` remain. They cycle endlessly. 3 robots remain.

## Input Format
- First line: An integer `n`, the number of robots (and batteries).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of batteries.

## Output Format
- Return a single integer representing the number of robots who cannot get a battery.

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
