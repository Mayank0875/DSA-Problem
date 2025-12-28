## Title
Movie Theater Popcorn

## Slug
movie-theater-popcorn

## Difficulty
Medium

## Description
Moviegoers want snacks. The counter has pre-filled Salted (0) and Sweet (1) popcorn buckets.

There are two types of buckets: **Salted** (represented by `0`) and **Sweet** (represented by `1`). Each moviegoer has a specific preference and will only accept one type of bucket.

The buckets are prepared in a **stack**, meaning only the top bucket is accessible at any time. The distribution process works as follows:
1. If the moviegoer at the front of the queue prefers the bucket currently on top of the stack, they take it and leave the queue.
2. If they do not like the top bucket, they move to the very back of the queue to wait for another turn.

This cycle continues until either all moviegoers are served, or the moviegoer at the front of the queue (and everyone else behind them) refuses the bucket currently on top of the stack.

Your task is to determine the number of moviegoers who are unable to receive a bucket.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front moviegoer (1) dislikes top bucket (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front moviegoer (1) dislikes top bucket (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front moviegoer (0) takes top bucket (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front moviegoer (0) dislikes top bucket (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all moviegoers find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top bucket is `1` (Sweet). Three moviegoers prefer Salted (`0`) and three prefer Sweet (`1`). After the Sweet moviegoers take their buckets, the stack has `0` (Salted) on top, but only moviegoers wanting `1` remain. They cycle endlessly. 3 moviegoers remain.

## Input Format
- First line: An integer `n`, the number of moviegoers (and buckets).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of buckets.

## Output Format
- Return a single integer representing the number of moviegoers who cannot get a bucket.

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
