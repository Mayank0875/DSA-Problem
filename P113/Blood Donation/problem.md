## Title
Blood Donation

## Slug
blood-donation

## Difficulty
Medium

## Description
Patients need blood. The blood bank has Type A (0) and Type B (1) bags stacked in the fridge.

There are two types of blood bags: **Type A** (represented by `0`) and **Type B** (represented by `1`). Each patient has a specific preference and will only accept one type of blood bag.

The blood bags are prepared in a **stack**, meaning only the top blood bag is accessible at any time. The distribution process works as follows:
1. If the patient at the front of the queue prefers the blood bag currently on top of the stack, they take it and leave the queue.
2. If they do not like the top blood bag, they move to the very back of the queue to wait for another turn.

This cycle continues until either all patients are served, or the patient at the front of the queue (and everyone else behind them) refuses the blood bag currently on top of the stack.

Your task is to determine the number of patients who are unable to receive a blood bag.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front patient (1) dislikes top blood bag (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front patient (1) dislikes top blood bag (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front patient (0) takes top blood bag (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front patient (0) dislikes top blood bag (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all patients find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top blood bag is `1` (Type B). Three patients prefer Type A (`0`) and three prefer Type B (`1`). After the Type B patients take their blood bags, the stack has `0` (Type A) on top, but only patients wanting `1` remain. They cycle endlessly. 3 patients remain.

## Input Format
- First line: An integer `n`, the number of patients (and blood bags).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of blood bags.

## Output Format
- Return a single integer representing the number of patients who cannot get a blood bag.

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
