## Title
Card Game Deal

## Slug
card-game-deal

## Difficulty
Medium

## Description
Players wait for a card deal. The dealer flips Red (0) and Black (1) cards from a deck.

There are two types of cards: **Red** (represented by `0`) and **Black** (represented by `1`). Each player has a specific preference and will only accept one type of card.

The cards are prepared in a **stack**, meaning only the top card is accessible at any time. The distribution process works as follows:
1. If the player at the front of the queue prefers the card currently on top of the stack, they take it and leave the queue.
2. If they do not like the top card, they move to the very back of the queue to wait for another turn.

This cycle continues until either all players are served, or the player at the front of the queue (and everyone else behind them) refuses the card currently on top of the stack.

Your task is to determine the number of players who are unable to receive a card.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front player (1) dislikes top card (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front player (1) dislikes top card (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front player (0) takes top card (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front player (0) dislikes top card (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all players find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top card is `1` (Black). Three players prefer Red (`0`) and three prefer Black (`1`). After the Black players take their cards, the stack has `0` (Red) on top, but only players wanting `1` remain. They cycle endlessly. 3 players remain.

## Input Format
- First line: An integer `n`, the number of players (and cards).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of cards.

## Output Format
- Return a single integer representing the number of players who cannot get a card.

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
