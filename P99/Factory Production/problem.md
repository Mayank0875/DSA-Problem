## Title
Factory Production

## Slug
factory-production

## Difficulty
Hard

## Description
Managers assign tasks. Tasks output materials required for the next specific task.

Manager and Union are playing a strategic game using a task queue $p$ of length $n$. The game starts with a output of 0.

The players take turns, with Manager moving first. On each turn, a player chooses an integer $x$ from the task queue that has not been chosen before.
- If it is Manager's turn, the chosen value $x$ is **added** to the output.
- If it is Union's turn, the chosen value $x$ is **subtracted** from the output.

The rules for choosing $x$ are:
1. On the very first move of the game, Manager may choose **any** unselected task from the task queue.
2. On every move after the first:
   - Let $m$ be the index of the task chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected task.

The game continues until all tasks of the task queue have been chosen.

Manager plays optimally to **maximize** the final output, while Union plays optimally to **minimize** it.

Your task is to compute the final output assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final output is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final output is 1.

## Input Format
- The first line contains an integer $n$ (length of task queue).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final output on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
