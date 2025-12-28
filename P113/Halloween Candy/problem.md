## Title
Halloween Candy

## Slug
halloween-candy

## Difficulty
Medium

## Description
Trick-or-treaters grab candy. The bowl has Chocolate (0) and Gummy (1).

There are two types of candies: **Chocolate** (represented by `0`) and **Gummy** (represented by `1`). Each kid has a specific preference and will only accept one type of candy.

The candies are prepared in a **stack**, meaning only the top candy is accessible at any time. The distribution process works as follows:
1. If the kid at the front of the queue prefers the candy currently on top of the stack, they take it and leave the queue.
2. If they do not like the top candy, they move to the very back of the queue to wait for another turn.

This cycle continues until either all kids are served, or the kid at the front of the queue (and everyone else behind them) refuses the candy currently on top of the stack.

Your task is to determine the number of kids who are unable to receive a candy.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front kid (1) dislikes top candy (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front kid (1) dislikes top candy (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front kid (0) takes top candy (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front kid (0) dislikes top candy (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all kids find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top candy is `1` (Gummy). Three kids prefer Chocolate (`0`) and three prefer Gummy (`1`). After the Gummy kids take their candies, the stack has `0` (Chocolate) on top, but only kids wanting `1` remain. They cycle endlessly. 3 kids remain.

## Input Format
- First line: An integer `n`, the number of kids (and candies).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of candies.

## Output Format
- Return a single integer representing the number of kids who cannot get a candy.

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
