## Title
Hotel Key Cards

## Slug
hotel-key-cards

## Difficulty
Medium

## Description
Guests check in. The receptionist has Standard (0) and Suite (1) key cards in a pile.

There are two types of cards: **Standard** (represented by `0`) and **Suite** (represented by `1`). Each guest has a specific preference and will only accept one type of card.

The cards are prepared in a **stack**, meaning only the top card is accessible at any time. The distribution process works as follows:
1. If the guest at the front of the queue prefers the card currently on top of the stack, they take it and leave the queue.
2. If they do not like the top card, they move to the very back of the queue to wait for another turn.

This cycle continues until either all guests are served, or the guest at the front of the queue (and everyone else behind them) refuses the card currently on top of the stack.

Your task is to determine the number of guests who are unable to receive a card.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front guest (1) dislikes top card (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front guest (1) dislikes top card (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front guest (0) takes top card (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front guest (0) dislikes top card (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all guests find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top card is `1` (Suite). Three guests prefer Standard (`0`) and three prefer Suite (`1`). After the Suite guests take their cards, the stack has `0` (Standard) on top, but only guests wanting `1` remain. They cycle endlessly. 3 guests remain.

## Input Format
- First line: An integer `n`, the number of guests (and cards).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of cards.

## Output Format
- Return a single integer representing the number of guests who cannot get a card.

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
