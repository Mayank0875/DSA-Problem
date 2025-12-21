## Title
Magical Duel

## Slug
magical-duel

## Difficulty
Hard

## Description
Wizards cast spells from a spellbook where spells trigger subsequent spells.

Gandalf and Saruman are playing a strategic game using a spell sequence $p$ of length $n$. The game starts with a magic power of 0.

The players take turns, with Gandalf moving first. On each turn, a player chooses an integer $x$ from the spell sequence that has not been chosen before.
- If it is Gandalf's turn, the chosen value $x$ is **added** to the magic power.
- If it is Saruman's turn, the chosen value $x$ is **subtracted** from the magic power.

The rules for choosing $x$ are:
1. On the very first move of the game, Gandalf may choose **any** unselected spell from the spell sequence.
2. On every move after the first:
   - Let $m$ be the index of the spell chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected spell.

The game continues until all spells of the spell sequence have been chosen.

Gandalf plays optimally to **maximize** the final magic power, while Saruman plays optimally to **minimize** it.

Your task is to compute the final magic power assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final magic power is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final magic power is 1.

## Input Format
- The first line contains an integer $n$ (length of spell sequence).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final magic power on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
