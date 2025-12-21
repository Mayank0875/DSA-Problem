## Title
Mining Veins

## Slug
mining-veins

## Difficulty
Hard

## Description
Miners follow ore veins. A vein leads directly to a specific deposit.

Dwarf and Goblin are playing a strategic game using a deposit map $p$ of length $n$. The game starts with a ore mined of 0.

The players take turns, with Dwarf moving first. On each turn, a player chooses an integer $x$ from the deposit map that has not been chosen before.
- If it is Dwarf's turn, the chosen value $x$ is **added** to the ore mined.
- If it is Goblin's turn, the chosen value $x$ is **subtracted** from the ore mined.

The rules for choosing $x$ are:
1. On the very first move of the game, Dwarf may choose **any** unselected deposit from the deposit map.
2. On every move after the first:
   - Let $m$ be the index of the deposit chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected deposit.

The game continues until all deposits of the deposit map have been chosen.

Dwarf plays optimally to **maximize** the final ore mined, while Goblin plays optimally to **minimize** it.

Your task is to compute the final ore mined assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final ore mined is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final ore mined is 1.

## Input Format
- The first line contains an integer $n$ (length of deposit map).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final ore mined on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
