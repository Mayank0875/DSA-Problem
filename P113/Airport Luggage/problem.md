## Title
Airport Luggage

## Slug
airport-luggage

## Difficulty
Medium

## Description
Travelers wait at the carousel. Bags are Hard-shell (0) or Soft-shell (1).

There are two types of bags: **Hard-shell** (represented by `0`) and **Soft-shell** (represented by `1`). Each traveler has a specific preference and will only accept one type of bag.

The bags are prepared in a **stack**, meaning only the top bag is accessible at any time. The distribution process works as follows:
1. If the traveler at the front of the queue prefers the bag currently on top of the stack, they take it and leave the queue.
2. If they do not like the top bag, they move to the very back of the queue to wait for another turn.

This cycle continues until either all travelers are served, or the traveler at the front of the queue (and everyone else behind them) refuses the bag currently on top of the stack.

Your task is to determine the number of travelers who are unable to receive a bag.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front traveler (1) dislikes top bag (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front traveler (1) dislikes top bag (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front traveler (0) takes top bag (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front traveler (0) dislikes top bag (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all travelers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top bag is `1` (Soft-shell). Three travelers prefer Hard-shell (`0`) and three prefer Soft-shell (`1`). After the Soft-shell travelers take their bags, the stack has `0` (Hard-shell) on top, but only travelers wanting `1` remain. They cycle endlessly. 3 travelers remain.

## Input Format
- First line: An integer `n`, the number of travelers (and bags).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of bags.

## Output Format
- Return a single integer representing the number of travelers who cannot get a bag.

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
