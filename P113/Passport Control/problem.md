## Title
Passport Control

## Slug
passport-control

## Difficulty
Medium

## Description
Passengers queue at customs. The officer stamps Domestic (0) or International (1) passports based on the stamp stack.

There are two types of stamps: **Domestic** (represented by `0`) and **International** (represented by `1`). Each passenger has a specific preference and will only accept one type of stamp.

The stamps are prepared in a **stack**, meaning only the top stamp is accessible at any time. The distribution process works as follows:
1. If the passenger at the front of the queue prefers the stamp currently on top of the stack, they take it and leave the queue.
2. If they do not like the top stamp, they move to the very back of the queue to wait for another turn.

This cycle continues until either all passengers are served, or the passenger at the front of the queue (and everyone else behind them) refuses the stamp currently on top of the stack.

Your task is to determine the number of passengers who are unable to receive a stamp.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front passenger (1) dislikes top stamp (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front passenger (1) dislikes top stamp (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front passenger (0) takes top stamp (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front passenger (0) dislikes top stamp (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all passengers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top stamp is `1` (International). Three passengers prefer Domestic (`0`) and three prefer International (`1`). After the International passengers take their stamps, the stack has `0` (Domestic) on top, but only passengers wanting `1` remain. They cycle endlessly. 3 passengers remain.

## Input Format
- First line: An integer `n`, the number of passengers (and stamps).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of stamps.

## Output Format
- Return a single integer representing the number of passengers who cannot get a stamp.

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
