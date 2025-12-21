## Title
Quest Chain

## Slug
quest-chain

## Difficulty
Hard

## Description
Gamers complete quests. Completing one unlocks a specific follow-up.

Hero and Villain are playing a strategic game using a quest log $p$ of length $n$. The game starts with a XP earned of 0.

The players take turns, with Hero moving first. On each turn, a player chooses an integer $x$ from the quest log that has not been chosen before.
- If it is Hero's turn, the chosen value $x$ is **added** to the XP earned.
- If it is Villain's turn, the chosen value $x$ is **subtracted** from the XP earned.

The rules for choosing $x$ are:
1. On the very first move of the game, Hero may choose **any** unselected quest from the quest log.
2. On every move after the first:
   - Let $m$ be the index of the quest chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected quest.

The game continues until all quests of the quest log have been chosen.

Hero plays optimally to **maximize** the final XP earned, while Villain plays optimally to **minimize** it.

Your task is to compute the final XP earned assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final XP earned is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final XP earned is 1.

## Input Format
- The first line contains an integer $n$ (length of quest log).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final XP earned on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
