## Title
Political Debate

## Slug
political-debate

## Difficulty
Hard

## Description
Candidates select talking points. One point naturally leads to another.

Candidate A and Candidate B are playing a strategic game using a topic list $p$ of length $n$. The game starts with a poll rating of 0.

The players take turns, with Candidate A moving first. On each turn, a player chooses an integer $x$ from the topic list that has not been chosen before.
- If it is Candidate A's turn, the chosen value $x$ is **added** to the poll rating.
- If it is Candidate B's turn, the chosen value $x$ is **subtracted** from the poll rating.

The rules for choosing $x$ are:
1. On the very first move of the game, Candidate A may choose **any** unselected topic from the topic list.
2. On every move after the first:
   - Let $m$ be the index of the topic chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected topic.

The game continues until all topics of the topic list have been chosen.

Candidate A plays optimally to **maximize** the final poll rating, while Candidate B plays optimally to **minimize** it.

Your task is to compute the final poll rating assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final poll rating is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final poll rating is 1.

## Input Format
- The first line contains an integer $n$ (length of topic list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final poll rating on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
