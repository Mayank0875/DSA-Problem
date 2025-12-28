## Title
Tech Support Tickets

## Slug
tech-support-tickets

## Difficulty
Medium

## Description
Technicians pick tickets from a stack. Tickets are either Hardware (0) or Software (1) issues. Techs specialize.

There are two types of tickets: **Hardware** (represented by `0`) and **Software** (represented by `1`). Each technician has a specific preference and will only accept one type of ticket.

The tickets are prepared in a **stack**, meaning only the top ticket is accessible at any time. The distribution process works as follows:
1. If the technician at the front of the queue prefers the ticket currently on top of the stack, they take it and leave the queue.
2. If they do not like the top ticket, they move to the very back of the queue to wait for another turn.

This cycle continues until either all technicians are served, or the technician at the front of the queue (and everyone else behind them) refuses the ticket currently on top of the stack.

Your task is to determine the number of technicians who are unable to receive a ticket.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front technician (1) dislikes top ticket (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front technician (1) dislikes top ticket (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front technician (0) takes top ticket (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front technician (0) dislikes top ticket (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all technicians find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top ticket is `1` (Software). Three technicians prefer Hardware (`0`) and three prefer Software (`1`). After the Software technicians take their tickets, the stack has `0` (Hardware) on top, but only technicians wanting `1` remain. They cycle endlessly. 3 technicians remain.

## Input Format
- First line: An integer `n`, the number of technicians (and tickets).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of tickets.

## Output Format
- Return a single integer representing the number of technicians who cannot get a ticket.

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
