## Title
Garden Center

## Slug
garden-center

## Difficulty
Medium

## Description
Gardeners buy seeds. The rack dispenses Vegetable (0) and Flower (1) packets.

There are two types of packets: **Vegetable** (represented by `0`) and **Flower** (represented by `1`). Each gardener has a specific preference and will only accept one type of packet.

The packets are prepared in a **stack**, meaning only the top packet is accessible at any time. The distribution process works as follows:
1. If the gardener at the front of the queue prefers the packet currently on top of the stack, they take it and leave the queue.
2. If they do not like the top packet, they move to the very back of the queue to wait for another turn.

This cycle continues until either all gardeners are served, or the gardener at the front of the queue (and everyone else behind them) refuses the packet currently on top of the stack.

Your task is to determine the number of gardeners who are unable to receive a packet.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front gardener (1) dislikes top packet (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front gardener (1) dislikes top packet (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front gardener (0) takes top packet (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front gardener (0) dislikes top packet (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all gardeners find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top packet is `1` (Flower). Three gardeners prefer Vegetable (`0`) and three prefer Flower (`1`). After the Flower gardeners take their packets, the stack has `0` (Vegetable) on top, but only gardeners wanting `1` remain. They cycle endlessly. 3 gardeners remain.

## Input Format
- First line: An integer `n`, the number of gardeners (and packets).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of packets.

## Output Format
- Return a single integer representing the number of gardeners who cannot get a packet.

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
