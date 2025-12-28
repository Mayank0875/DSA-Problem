## Title
Coin Exchange

## Slug
coin-exchange

## Difficulty
Medium

## Description
Collectors wait for rare coins. The bank teller has Silver (0) and Gold (1) coins in a tube.

There are two types of coins: **Silver** (represented by `0`) and **Gold** (represented by `1`). Each collector has a specific preference and will only accept one type of coin.

The coins are prepared in a **stack**, meaning only the top coin is accessible at any time. The distribution process works as follows:
1. If the collector at the front of the queue prefers the coin currently on top of the stack, they take it and leave the queue.
2. If they do not like the top coin, they move to the very back of the queue to wait for another turn.

This cycle continues until either all collectors are served, or the collector at the front of the queue (and everyone else behind them) refuses the coin currently on top of the stack.

Your task is to determine the number of collectors who are unable to receive a coin.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front collector (1) dislikes top coin (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front collector (1) dislikes top coin (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front collector (0) takes top coin (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front collector (0) dislikes top coin (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all collectors find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top coin is `1` (Gold). Three collectors prefer Silver (`0`) and three prefer Gold (`1`). After the Gold collectors take their coins, the stack has `0` (Silver) on top, but only collectors wanting `1` remain. They cycle endlessly. 3 collectors remain.

## Input Format
- First line: An integer `n`, the number of collectors (and coins).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of coins.

## Output Format
- Return a single integer representing the number of collectors who cannot get a coin.

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
