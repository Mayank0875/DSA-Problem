## Title
Spaceport Ticketing

## Slug
spaceport-ticketing

## Difficulty
Medium

## Description
Travelers queue at a spaceport. Tickets are issued for two destinations: Mars (0) and Venus (1).

There are two types of tickets: **Mars Tickets** (represented by `0`) and **Venus Tickets** (represented by `1`). Each traveler has a specific preference and will only accept one type of ticket.

The tickets are prepared in a **stack**, meaning only the top ticket is accessible at any time. The distribution process works as follows:
1. If the traveler at the front of the queue prefers the ticket currently on top of the stack, they take it and leave the queue.
2. If they do not like the top ticket, they move to the very back of the queue to wait for another turn.

This cycle continues until either all travelers are served, or the traveler at the front of the queue (and everyone else behind them) refuses the ticket currently on top of the stack.

Your task is to determine the number of travelers who are unable to receive a ticket.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front traveler (1) dislikes top ticket (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front traveler (1) dislikes top ticket (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front traveler (0) takes top ticket (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front traveler (0) dislikes top ticket (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all travelers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top ticket is `1` (Venus Tickets). Three travelers prefer Mars Tickets (`0`) and three prefer Venus Tickets (`1`). After the Venus Tickets travelers take their tickets, the stack has `0` (Mars Tickets) on top, but only travelers wanting `1` remain. They cycle endlessly. 3 travelers remain.

## Input Format
- First line: An integer `n`, the number of travelers (and tickets).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of tickets.

## Output Format
- Return a single integer representing the number of travelers who cannot get a ticket.

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
