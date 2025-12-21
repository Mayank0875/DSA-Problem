## Title
Time Travel Loop

## Slug
time-travel-loop

## Difficulty
Hard

## Description
Travelers jump to timelines. Each timeline dictates the next jump coordinates.

Traveler and Paradox are playing a strategic game using a timeline graph $p$ of length $n$. The game starts with a chronal energy of 0.

The players take turns, with Traveler moving first. On each turn, a player chooses an integer $x$ from the timeline graph that has not been chosen before.
- If it is Traveler's turn, the chosen value $x$ is **added** to the chronal energy.
- If it is Paradox's turn, the chosen value $x$ is **subtracted** from the chronal energy.

The rules for choosing $x$ are:
1. On the very first move of the game, Traveler may choose **any** unselected timeline from the timeline graph.
2. On every move after the first:
   - Let $m$ be the index of the timeline chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected timeline.

The game continues until all timelines of the timeline graph have been chosen.

Traveler plays optimally to **maximize** the final chronal energy, while Paradox plays optimally to **minimize** it.

Your task is to compute the final chronal energy assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final chronal energy is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final chronal energy is 1.

## Input Format
- The first line contains an integer $n$ (length of timeline graph).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final chronal energy on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
