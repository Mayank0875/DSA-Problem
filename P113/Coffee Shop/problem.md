## Title
Coffee Shop

## Slug
coffee-shop

## Difficulty
Medium

## Description
Baristas need cups. The stack has Paper (0) and Ceramic (1) cups.

There are two types of cups: **Paper** (represented by `0`) and **Ceramic** (represented by `1`). Each barista has a specific preference and will only accept one type of cup.

The cups are prepared in a **stack**, meaning only the top cup is accessible at any time. The distribution process works as follows:
1. If the barista at the front of the queue prefers the cup currently on top of the stack, they take it and leave the queue.
2. If they do not like the top cup, they move to the very back of the queue to wait for another turn.

This cycle continues until either all baristas are served, or the barista at the front of the queue (and everyone else behind them) refuses the cup currently on top of the stack.

Your task is to determine the number of baristas who are unable to receive a cup.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front barista (1) dislikes top cup (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front barista (1) dislikes top cup (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front barista (0) takes top cup (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front barista (0) dislikes top cup (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all baristas find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top cup is `1` (Ceramic). Three baristas prefer Paper (`0`) and three prefer Ceramic (`1`). After the Ceramic baristas take their cups, the stack has `0` (Paper) on top, but only baristas wanting `1` remain. They cycle endlessly. 3 baristas remain.

## Input Format
- First line: An integer `n`, the number of baristas (and cups).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of cups.

## Output Format
- Return a single integer representing the number of baristas who cannot get a cup.

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
