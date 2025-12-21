## Title
Viral Spread

## Slug
viral-spread

## Difficulty
Hard

## Description
Doctors treat patients. Contact tracing points to the next infected person.

Doctor and Virus are playing a strategic game using a patient list $p$ of length $n$. The game starts with a health score of 0.

The players take turns, with Doctor moving first. On each turn, a player chooses an integer $x$ from the patient list that has not been chosen before.
- If it is Doctor's turn, the chosen value $x$ is **added** to the health score.
- If it is Virus's turn, the chosen value $x$ is **subtracted** from the health score.

The rules for choosing $x$ are:
1. On the very first move of the game, Doctor may choose **any** unselected patient from the patient list.
2. On every move after the first:
   - Let $m$ be the index of the patient chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected patient.

The game continues until all patients of the patient list have been chosen.

Doctor plays optimally to **maximize** the final health score, while Virus plays optimally to **minimize** it.

Your task is to compute the final health score assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final health score is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final health score is 1.

## Input Format
- The first line contains an integer $n$ (length of patient list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final health score on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
