## Title
Music Festival

## Slug
music-festival

## Difficulty
Medium

## Description
Attendees get passes. The box has Day (0) and Weekend (1) passes.

There are two types of passes: **Day** (represented by `0`) and **Weekend** (represented by `1`). Each attendee has a specific preference and will only accept one type of pass.

The passes are prepared in a **stack**, meaning only the top pass is accessible at any time. The distribution process works as follows:
1. If the attendee at the front of the queue prefers the pass currently on top of the stack, they take it and leave the queue.
2. If they do not like the top pass, they move to the very back of the queue to wait for another turn.

This cycle continues until either all attendees are served, or the attendee at the front of the queue (and everyone else behind them) refuses the pass currently on top of the stack.

Your task is to determine the number of attendees who are unable to receive a pass.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front attendee (1) dislikes top pass (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front attendee (1) dislikes top pass (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front attendee (0) takes top pass (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front attendee (0) dislikes top pass (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all attendees find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top pass is `1` (Weekend). Three attendees prefer Day (`0`) and three prefer Weekend (`1`). After the Weekend attendees take their passes, the stack has `0` (Day) on top, but only attendees wanting `1` remain. They cycle endlessly. 3 attendees remain.

## Input Format
- First line: An integer `n`, the number of attendees (and passes).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of passes.

## Output Format
- Return a single integer representing the number of attendees who cannot get a pass.

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
