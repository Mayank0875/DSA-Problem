## Title
Legal Loopholes

## Slug
legal-loopholes

## Difficulty
Hard

## Description
Lawyers cite precedents. Each precedent refers to another specific case.

Defense and Prosecution are playing a strategic game using a case list $p$ of length $n$. The game starts with a case strength of 0.

The players take turns, with Defense moving first. On each turn, a player chooses an integer $x$ from the case list that has not been chosen before.
- If it is Defense's turn, the chosen value $x$ is **added** to the case strength.
- If it is Prosecution's turn, the chosen value $x$ is **subtracted** from the case strength.

The rules for choosing $x$ are:
1. On the very first move of the game, Defense may choose **any** unselected precedent from the case list.
2. On every move after the first:
   - Let $m$ be the index of the precedent chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected precedent.

The game continues until all precedents of the case list have been chosen.

Defense plays optimally to **maximize** the final case strength, while Prosecution plays optimally to **minimize** it.

Your task is to compute the final case strength assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final case strength is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final case strength is 1.

## Input Format
- The first line contains an integer $n$ (length of case list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final case strength on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
