## Title
Chain Reaction

## Slug
chain-reaction

## Difficulty
Hard

## Description
Physicists split atoms. Fission triggers a specific neighbor atom.

Physicist and Entropy are playing a strategic game using a atom lattice $p$ of length $n$. The game starts with a energy release of 0.

The players take turns, with Physicist moving first. On each turn, a player chooses an integer $x$ from the atom lattice that has not been chosen before.
- If it is Physicist's turn, the chosen value $x$ is **added** to the energy release.
- If it is Entropy's turn, the chosen value $x$ is **subtracted** from the energy release.

The rules for choosing $x$ are:
1. On the very first move of the game, Physicist may choose **any** unselected atom from the atom lattice.
2. On every move after the first:
   - Let $m$ be the index of the atom chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected atom.

The game continues until all atoms of the atom lattice have been chosen.

Physicist plays optimally to **maximize** the final energy release, while Entropy plays optimally to **minimize** it.

Your task is to compute the final energy release assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final energy release is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final energy release is 1.

## Input Format
- The first line contains an integer $n$ (length of atom lattice).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final energy release on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
