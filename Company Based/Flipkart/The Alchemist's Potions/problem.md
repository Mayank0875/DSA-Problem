## Title

The Alchemist's Potions

## Slug

the-alchemists-potions

## Difficulty

Easy

## Description

In a prestigious magic academy, young apprentices are waiting in a queue to collect their daily mana potions. There are two types of potions available: **Fire Potions** (represented by `0`) and **Ice Potions** (represented by `1`). Each apprentice has a specific affinity and will only accept one type of potion.

The potions are prepared in a **stack**, meaning only the top potion is accessible at any time. The distribution process works as follows:
1. If the apprentice at the front of the queue prefers the potion currently on top of the stack, they take it and leave the queue.
2. If they do not like the top potion, they move to the very back of the queue to wait for another turn.

This cycle continues until either all apprentices are served, or the apprentice at the front of the queue (and everyone else behind them) refuses the potion currently on top of the stack.

Your task is to determine the number of apprentices who are unable to receive a potion.

## Examples

### 1

#### Input

4 
1 1 0 0
0 1 0 1

#### Output

0

#### Explanation

* Front apprentice (1) dislikes top potion (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front apprentice (1) dislikes top potion (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front apprentice (0) takes top potion (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front apprentice (0) dislikes top potion (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all apprentices find their preferred match.
    
### 2

#### Input

6 
1 1 1 0 0 1 
1 0 0 0 1 1

#### Output

3

#### Explanation

The top potion is `1` (Ice). Three apprentices prefer Fire `0` and three prefer Ice `1`. After the Ice apprentices take their potions, the stack has `0` (Fire) on top, but only apprentices wanting `1` remain. They cycle endlessly, unable to eat. 3 apprentices remain.
  

## Input Format  

- First line: An integer `n`, the number of apprentices (and potions).
- Second line: `n` space-separated integers representing the `apprentices` queue preferences.
- Third line: `n` space-separated integers representing the `potions` stack.

## Output Format  

- Return a single integer representing the number of apprentices who cannot get a potion.
  

## Constraints  

- 1 ≤ n ≤ 100
- `apprentices[i]` is `0` or `1`.
- `potions[i]` is `0` or `1`.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, queue