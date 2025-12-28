## Title
Pharmacy Counter

## Slug
pharmacy-counter

## Difficulty
Medium

## Description
Patients pick up prescriptions. The bin has Tablets (0) and Liquids (1).

There are two types of meds: **Tablets** (represented by `0`) and **Liquids** (represented by `1`). Each patient has a specific preference and will only accept one type of med.

The meds are prepared in a **stack**, meaning only the top med is accessible at any time. The distribution process works as follows:
1. If the patient at the front of the queue prefers the med currently on top of the stack, they take it and leave the queue.
2. If they do not like the top med, they move to the very back of the queue to wait for another turn.

This cycle continues until either all patients are served, or the patient at the front of the queue (and everyone else behind them) refuses the med currently on top of the stack.

Your task is to determine the number of patients who are unable to receive a med.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front patient (1) dislikes top med (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front patient (1) dislikes top med (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front patient (0) takes top med (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front patient (0) dislikes top med (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all patients find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top med is `1` (Liquids). Three patients prefer Tablets (`0`) and three prefer Liquids (`1`). After the Liquids patients take their meds, the stack has `0` (Tablets) on top, but only patients wanting `1` remain. They cycle endlessly. 3 patients remain.

## Input Format
- First line: An integer `n`, the number of patients (and meds).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of meds.

## Output Format
- Return a single integer representing the number of patients who cannot get a med.

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
