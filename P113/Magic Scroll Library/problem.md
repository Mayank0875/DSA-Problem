## Title
Magic Scroll Library

## Slug
magic-scroll-library

## Difficulty
Medium

## Description
Wizards need spells. The archive stack has Fire (0) and Ice (1) scrolls.

There are two types of scrolls: **Fire** (represented by `0`) and **Ice** (represented by `1`). Each wizard has a specific preference and will only accept one type of scroll.

The scrolls are prepared in a **stack**, meaning only the top scroll is accessible at any time. The distribution process works as follows:
1. If the wizard at the front of the queue prefers the scroll currently on top of the stack, they take it and leave the queue.
2. If they do not like the top scroll, they move to the very back of the queue to wait for another turn.

This cycle continues until either all wizards are served, or the wizard at the front of the queue (and everyone else behind them) refuses the scroll currently on top of the stack.

Your task is to determine the number of wizards who are unable to receive a scroll.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front wizard (1) dislikes top scroll (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front wizard (1) dislikes top scroll (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front wizard (0) takes top scroll (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front wizard (0) dislikes top scroll (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all wizards find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top scroll is `1` (Ice). Three wizards prefer Fire (`0`) and three prefer Ice (`1`). After the Ice wizards take their scrolls, the stack has `0` (Fire) on top, but only wizards wanting `1` remain. They cycle endlessly. 3 wizards remain.

## Input Format
- First line: An integer `n`, the number of wizards (and scrolls).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of scrolls.

## Output Format
- Return a single integer representing the number of wizards who cannot get a scroll.

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
