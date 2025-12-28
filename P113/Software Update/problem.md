## Title
Software Update

## Slug
software-update

## Difficulty
Medium

## Description
Devices queue for updates. The server pushes Security (0) and Feature (1) patches sequentially.

There are two types of patches: **Security** (represented by `0`) and **Feature** (represented by `1`). Each device has a specific preference and will only accept one type of patch.

The patches are prepared in a **stack**, meaning only the top patch is accessible at any time. The distribution process works as follows:
1. If the device at the front of the queue prefers the patch currently on top of the stack, they take it and leave the queue.
2. If they do not like the top patch, they move to the very back of the queue to wait for another turn.

This cycle continues until either all devices are served, or the device at the front of the queue (and everyone else behind them) refuses the patch currently on top of the stack.

Your task is to determine the number of devices who are unable to receive a patch.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front device (1) dislikes top patch (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front device (1) dislikes top patch (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front device (0) takes top patch (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front device (0) dislikes top patch (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all devices find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top patch is `1` (Feature). Three devices prefer Security (`0`) and three prefer Feature (`1`). After the Feature devices take their patches, the stack has `0` (Security) on top, but only devices wanting `1` remain. They cycle endlessly. 3 devices remain.

## Input Format
- First line: An integer `n`, the number of devices (and patches).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of patches.

## Output Format
- Return a single integer representing the number of devices who cannot get a patch.

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
