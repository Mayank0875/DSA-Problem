## Title
Factory Assembly

## Slug
factory-assembly

## Difficulty
Medium

## Description
Robotic arms wait for parts. The conveyor belt delivers Bolts (0) and Nuts (1) in a vertical feeder.

There are two types of parts: **Bolts** (represented by `0`) and **Nuts** (represented by `1`). Each arm has a specific preference and will only accept one type of part.

The parts are prepared in a **stack**, meaning only the top part is accessible at any time. The distribution process works as follows:
1. If the arm at the front of the queue prefers the part currently on top of the stack, they take it and leave the queue.
2. If they do not like the top part, they move to the very back of the queue to wait for another turn.

This cycle continues until either all arms are served, or the arm at the front of the queue (and everyone else behind them) refuses the part currently on top of the stack.

Your task is to determine the number of arms who are unable to receive a part.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front arm (1) dislikes top part (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front arm (1) dislikes top part (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front arm (0) takes top part (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front arm (0) dislikes top part (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all arms find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top part is `1` (Nuts). Three arms prefer Bolts (`0`) and three prefer Nuts (`1`). After the Nuts arms take their parts, the stack has `0` (Bolts) on top, but only arms wanting `1` remain. They cycle endlessly. 3 arms remain.

## Input Format
- First line: An integer `n`, the number of arms (and parts).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of parts.

## Output Format
- Return a single integer representing the number of arms who cannot get a part.

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
