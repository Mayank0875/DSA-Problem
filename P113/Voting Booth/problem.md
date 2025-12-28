## Title
Voting Booth

## Slug
voting-booth

## Difficulty
Medium

## Description
Voters need ballots. The machine prints Paper (0) and Electronic (1) tokens.

There are two types of ballots: **Paper** (represented by `0`) and **Electronic** (represented by `1`). Each voter has a specific preference and will only accept one type of ballot.

The ballots are prepared in a **stack**, meaning only the top ballot is accessible at any time. The distribution process works as follows:
1. If the voter at the front of the queue prefers the ballot currently on top of the stack, they take it and leave the queue.
2. If they do not like the top ballot, they move to the very back of the queue to wait for another turn.

This cycle continues until either all voters are served, or the voter at the front of the queue (and everyone else behind them) refuses the ballot currently on top of the stack.

Your task is to determine the number of voters who are unable to receive a ballot.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front voter (1) dislikes top ballot (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front voter (1) dislikes top ballot (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front voter (0) takes top ballot (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front voter (0) dislikes top ballot (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all voters find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top ballot is `1` (Electronic). Three voters prefer Paper (`0`) and three prefer Electronic (`1`). After the Electronic voters take their ballots, the stack has `0` (Paper) on top, but only voters wanting `1` remain. They cycle endlessly. 3 voters remain.

## Input Format
- First line: An integer `n`, the number of voters (and ballots).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of ballots.

## Output Format
- Return a single integer representing the number of voters who cannot get a ballot.

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
