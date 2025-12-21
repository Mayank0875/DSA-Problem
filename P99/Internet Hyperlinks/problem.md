## Title
Internet Hyperlinks

## Slug
internet-hyperlinks

## Difficulty
Hard

## Description
Users click links. A page redirects to a specific URL.

Surfer and Adbot are playing a strategic game using a web graph $p$ of length $n$. The game starts with a info gain of 0.

The players take turns, with Surfer moving first. On each turn, a player chooses an integer $x$ from the web graph that has not been chosen before.
- If it is Surfer's turn, the chosen value $x$ is **added** to the info gain.
- If it is Adbot's turn, the chosen value $x$ is **subtracted** from the info gain.

The rules for choosing $x$ are:
1. On the very first move of the game, Surfer may choose **any** unselected page from the web graph.
2. On every move after the first:
   - Let $m$ be the index of the page chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected page.

The game continues until all pages of the web graph have been chosen.

Surfer plays optimally to **maximize** the final info gain, while Adbot plays optimally to **minimize** it.

Your task is to compute the final info gain assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final info gain is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final info gain is 1.

## Input Format
- The first line contains an integer $n$ (length of web graph).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final info gain on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
