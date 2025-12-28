## Title
Train Station Turnstile

## Slug
train-station-turnstile

## Difficulty
Medium

## Description
Commuters tap cards. The machine issues Entry (0) or Exit (1) tokens.

There are two types of tokens: **Entry** (represented by `0`) and **Exit** (represented by `1`). Each commuter has a specific preference and will only accept one type of token.

The tokens are prepared in a **stack**, meaning only the top token is accessible at any time. The distribution process works as follows:
1. If the commuter at the front of the queue prefers the token currently on top of the stack, they take it and leave the queue.
2. If they do not like the top token, they move to the very back of the queue to wait for another turn.

This cycle continues until either all commuters are served, or the commuter at the front of the queue (and everyone else behind them) refuses the token currently on top of the stack.

Your task is to determine the number of commuters who are unable to receive a token.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front commuter (1) dislikes top token (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front commuter (1) dislikes top token (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front commuter (0) takes top token (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front commuter (0) dislikes top token (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all commuters find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top token is `1` (Exit). Three commuters prefer Entry (`0`) and three prefer Exit (`1`). After the Exit commuters take their tokens, the stack has `0` (Entry) on top, but only commuters wanting `1` remain. They cycle endlessly. 3 commuters remain.

## Input Format
- First line: An integer `n`, the number of commuters (and tokens).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of tokens.

## Output Format
- Return a single integer representing the number of commuters who cannot get a token.

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
