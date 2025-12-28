## Title
Food Bank

## Slug
food-bank

## Difficulty
Medium

## Description
People wait for food parcels. The distribution center has Canned Goods (0) and Fresh Produce (1) boxes stacked.

There are two types of parcels: **Canned Goods** (represented by `0`) and **Fresh Produce** (represented by `1`). Each person has a specific preference and will only accept one type of parcel.

The parcels are prepared in a **stack**, meaning only the top parcel is accessible at any time. The distribution process works as follows:
1. If the person at the front of the queue prefers the parcel currently on top of the stack, they take it and leave the queue.
2. If they do not like the top parcel, they move to the very back of the queue to wait for another turn.

This cycle continues until either all people are served, or the person at the front of the queue (and everyone else behind them) refuses the parcel currently on top of the stack.

Your task is to determine the number of people who are unable to receive a parcel.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front person (1) dislikes top parcel (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front person (1) dislikes top parcel (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front person (0) takes top parcel (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front person (0) dislikes top parcel (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all people find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top parcel is `1` (Fresh Produce). Three people prefer Canned Goods (`0`) and three prefer Fresh Produce (`1`). After the Fresh Produce people take their parcels, the stack has `0` (Canned Goods) on top, but only people wanting `1` remain. They cycle endlessly. 3 people remain.

## Input Format
- First line: An integer `n`, the number of people (and parcels).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of parcels.

## Output Format
- Return a single integer representing the number of people who cannot get a parcel.

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
