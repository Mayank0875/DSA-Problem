## Title
Circuit Breaker

## Slug
circuit-breaker

## Difficulty
Hard

## Description
Engineers activate switches. Wiring forces the next switch choice unless the circuit breaks.

Sparky and Shorty are playing a strategic game using a switch board $p$ of length $n$. The game starts with a voltage of 0.

The players take turns, with Sparky moving first. On each turn, a player chooses an integer $x$ from the switch board that has not been chosen before.
- If it is Sparky's turn, the chosen value $x$ is **added** to the voltage.
- If it is Shorty's turn, the chosen value $x$ is **subtracted** from the voltage.

The rules for choosing $x$ are:
1. On the very first move of the game, Sparky may choose **any** unselected switch from the switch board.
2. On every move after the first:
   - Let $m$ be the index of the switch chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected switch.

The game continues until all switches of the switch board have been chosen.

Sparky plays optimally to **maximize** the final voltage, while Shorty plays optimally to **minimize** it.

Your task is to compute the final voltage assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final voltage is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final voltage is 1.

## Input Format
- The first line contains an integer $n$ (length of switch board).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final voltage on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
