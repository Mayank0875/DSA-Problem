## Title
Concert Wristbands

## Slug
concert-wristbands

## Difficulty
Medium

## Description
Fans line up for wristbands. The box contains VIP (0) and General (1) bands mixed in a stack.

There are two types of wristbands: **VIP** (represented by `0`) and **General** (represented by `1`). Each fan has a specific preference and will only accept one type of wristband.

The wristbands are prepared in a **stack**, meaning only the top wristband is accessible at any time. The distribution process works as follows:
1. If the fan at the front of the queue prefers the wristband currently on top of the stack, they take it and leave the queue.
2. If they do not like the top wristband, they move to the very back of the queue to wait for another turn.

This cycle continues until either all fans are served, or the fan at the front of the queue (and everyone else behind them) refuses the wristband currently on top of the stack.

Your task is to determine the number of fans who are unable to receive a wristband.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front fan (1) dislikes top wristband (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front fan (1) dislikes top wristband (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front fan (0) takes top wristband (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front fan (0) dislikes top wristband (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all fans find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top wristband is `1` (General). Three fans prefer VIP (`0`) and three prefer General (`1`). After the General fans take their wristbands, the stack has `0` (VIP) on top, but only fans wanting `1` remain. They cycle endlessly. 3 fans remain.

## Input Format
- First line: An integer `n`, the number of fans (and wristbands).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of wristbands.

## Output Format
- Return a single integer representing the number of fans who cannot get a wristband.

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
