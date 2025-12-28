## Title
Warehouse Forklift

## Slug
warehouse-forklift

## Difficulty
Medium

## Description
Drivers need pallets. The stack has Wood (0) and Plastic (1) pallets.

There are two types of pallets: **Wood** (represented by `0`) and **Plastic** (represented by `1`). Each driver has a specific preference and will only accept one type of pallet.

The pallets are prepared in a **stack**, meaning only the top pallet is accessible at any time. The distribution process works as follows:
1. If the driver at the front of the queue prefers the pallet currently on top of the stack, they take it and leave the queue.
2. If they do not like the top pallet, they move to the very back of the queue to wait for another turn.

This cycle continues until either all drivers are served, or the driver at the front of the queue (and everyone else behind them) refuses the pallet currently on top of the stack.

Your task is to determine the number of drivers who are unable to receive a pallet.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front driver (1) dislikes top pallet (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front driver (1) dislikes top pallet (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front driver (0) takes top pallet (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front driver (0) dislikes top pallet (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all drivers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top pallet is `1` (Plastic). Three drivers prefer Wood (`0`) and three prefer Plastic (`1`). After the Plastic drivers take their pallets, the stack has `0` (Wood) on top, but only drivers wanting `1` remain. They cycle endlessly. 3 drivers remain.

## Input Format
- First line: An integer `n`, the number of drivers (and pallets).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of pallets.

## Output Format
- Return a single integer representing the number of drivers who cannot get a pallet.

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
