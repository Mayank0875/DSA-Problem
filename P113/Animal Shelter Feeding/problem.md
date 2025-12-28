## Title
Animal Shelter Feeding

## Slug
animal-shelter-feeding

## Difficulty
Medium

## Description
Animals wait for food bowls. Bowls contain either Wet Food (0) or Dry Kibble (1).

There are two types of bowls: **Wet Food** (represented by `0`) and **Dry Kibble** (represented by `1`). Each animal has a specific preference and will only accept one type of bowl.

The bowls are prepared in a **stack**, meaning only the top bowl is accessible at any time. The distribution process works as follows:
1. If the animal at the front of the queue prefers the bowl currently on top of the stack, they take it and leave the queue.
2. If they do not like the top bowl, they move to the very back of the queue to wait for another turn.

This cycle continues until either all animals are served, or the animal at the front of the queue (and everyone else behind them) refuses the bowl currently on top of the stack.

Your task is to determine the number of animals who are unable to receive a bowl.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front animal (1) dislikes top bowl (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front animal (1) dislikes top bowl (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front animal (0) takes top bowl (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front animal (0) dislikes top bowl (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all animals find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top bowl is `1` (Dry Kibble). Three animals prefer Wet Food (`0`) and three prefer Dry Kibble (`1`). After the Dry Kibble animals take their bowls, the stack has `0` (Wet Food) on top, but only animals wanting `1` remain. They cycle endlessly. 3 animals remain.

## Input Format
- First line: An integer `n`, the number of animals (and bowls).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of bowls.

## Output Format
- Return a single integer representing the number of animals who cannot get a bowl.

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
