## Title
Ancient Ritual

## Slug
ancient-ritual

## Difficulty
Hard

## Description
Priests light candles. The flame jumps to a specific next candle.

High Priest and Dark Spirit are playing a strategic game using a candle circle $p$ of length $n$. The game starts with a light level of 0.

The players take turns, with High Priest moving first. On each turn, a player chooses an integer $x$ from the candle circle that has not been chosen before.
- If it is High Priest's turn, the chosen value $x$ is **added** to the light level.
- If it is Dark Spirit's turn, the chosen value $x$ is **subtracted** from the light level.

The rules for choosing $x$ are:
1. On the very first move of the game, High Priest may choose **any** unselected candle from the candle circle.
2. On every move after the first:
   - Let $m$ be the index of the candle chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected candle.

The game continues until all candles of the candle circle have been chosen.

High Priest plays optimally to **maximize** the final light level, while Dark Spirit plays optimally to **minimize** it.

Your task is to compute the final light level assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final light level is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final light level is 1.

## Input Format
- The first line contains an integer $n$ (length of candle circle).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final light level on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
