## Title
Toy Drive

## Slug
toy-drive

## Difficulty
Medium

## Description
Families receive gifts. The sack has Dolls (0) and Trucks (1).

There are two types of toys: **Dolls** (represented by `0`) and **Trucks** (represented by `1`). Each family has a specific preference and will only accept one type of toy.

The toys are prepared in a **stack**, meaning only the top toy is accessible at any time. The distribution process works as follows:
1. If the family at the front of the queue prefers the toy currently on top of the stack, they take it and leave the queue.
2. If they do not like the top toy, they move to the very back of the queue to wait for another turn.

This cycle continues until either all families are served, or the family at the front of the queue (and everyone else behind them) refuses the toy currently on top of the stack.

Your task is to determine the number of families who are unable to receive a toy.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front family (1) dislikes top toy (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front family (1) dislikes top toy (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front family (0) takes top toy (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front family (0) dislikes top toy (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all families find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top toy is `1` (Trucks). Three families prefer Dolls (`0`) and three prefer Trucks (`1`). After the Trucks families take their toys, the stack has `0` (Dolls) on top, but only families wanting `1` remain. They cycle endlessly. 3 families remain.

## Input Format
- First line: An integer `n`, the number of families (and toys).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of toys.

## Output Format
- Return a single integer representing the number of families who cannot get a toy.

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
