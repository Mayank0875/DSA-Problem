## Title
Phone Charging Kiosk

## Slug
phone-charging-kiosk

## Difficulty
Medium

## Description
Users need cables. The kiosk dispenses USB-C (0) and Lightning (1) cables.

There are two types of cables: **USB-C** (represented by `0`) and **Lightning** (represented by `1`). Each user has a specific preference and will only accept one type of cable.

The cables are prepared in a **stack**, meaning only the top cable is accessible at any time. The distribution process works as follows:
1. If the user at the front of the queue prefers the cable currently on top of the stack, they take it and leave the queue.
2. If they do not like the top cable, they move to the very back of the queue to wait for another turn.

This cycle continues until either all users are served, or the user at the front of the queue (and everyone else behind them) refuses the cable currently on top of the stack.

Your task is to determine the number of users who are unable to receive a cable.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front user (1) dislikes top cable (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front user (1) dislikes top cable (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front user (0) takes top cable (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front user (0) dislikes top cable (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all users find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top cable is `1` (Lightning). Three users prefer USB-C (`0`) and three prefer Lightning (`1`). After the Lightning users take their cables, the stack has `0` (USB-C) on top, but only users wanting `1` remain. They cycle endlessly. 3 users remain.

## Input Format
- First line: An integer `n`, the number of users (and cables).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of cables.

## Output Format
- Return a single integer representing the number of users who cannot get a cable.

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
