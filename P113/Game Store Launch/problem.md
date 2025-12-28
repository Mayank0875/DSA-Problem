## Title
Game Store Launch

## Slug
game-store-launch

## Difficulty
Medium

## Description
Gamers want consoles. The stockroom releases Standard (0) and Digital (1) editions.

There are two types of consoles: **Standard** (represented by `0`) and **Digital** (represented by `1`). Each gamer has a specific preference and will only accept one type of console.

The consoles are prepared in a **stack**, meaning only the top console is accessible at any time. The distribution process works as follows:
1. If the gamer at the front of the queue prefers the console currently on top of the stack, they take it and leave the queue.
2. If they do not like the top console, they move to the very back of the queue to wait for another turn.

This cycle continues until either all gamers are served, or the gamer at the front of the queue (and everyone else behind them) refuses the console currently on top of the stack.

Your task is to determine the number of gamers who are unable to receive a console.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front gamer (1) dislikes top console (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front gamer (1) dislikes top console (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front gamer (0) takes top console (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front gamer (0) dislikes top console (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all gamers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top console is `1` (Digital). Three gamers prefer Standard (`0`) and three prefer Digital (`1`). After the Digital gamers take their consoles, the stack has `0` (Standard) on top, but only gamers wanting `1` remain. They cycle endlessly. 3 gamers remain.

## Input Format
- First line: An integer `n`, the number of gamers (and consoles).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of consoles.

## Output Format
- Return a single integer representing the number of gamers who cannot get a console.

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
