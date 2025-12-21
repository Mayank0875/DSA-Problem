## Title
Spy Network

## Slug
spy-network

## Difficulty
Hard

## Description
Agencies activate sleeper agents. Agents know the contact for exactly one other agent.

Agency and Mole are playing a strategic game using a agent list $p$ of length $n$. The game starts with a intel value of 0.

The players take turns, with Agency moving first. On each turn, a player chooses an integer $x$ from the agent list that has not been chosen before.
- If it is Agency's turn, the chosen value $x$ is **added** to the intel value.
- If it is Mole's turn, the chosen value $x$ is **subtracted** from the intel value.

The rules for choosing $x$ are:
1. On the very first move of the game, Agency may choose **any** unselected agent from the agent list.
2. On every move after the first:
   - Let $m$ be the index of the agent chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected agent.

The game continues until all agents of the agent list have been chosen.

Agency plays optimally to **maximize** the final intel value, while Mole plays optimally to **minimize** it.

Your task is to compute the final intel value assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final intel value is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final intel value is 1.

## Input Format
- The first line contains an integer $n$ (length of agent list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final intel value on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
