## Title
Book Cipher

## Slug
book-cipher

## Difficulty
Hard

## Description
Spies decode words. The cipher text directs to the next word index.

Decoder and Encoder are playing a strategic game using a page text $p$ of length $n$. The game starts with a message clarity of 0.

The players take turns, with Decoder moving first. On each turn, a player chooses an integer $x$ from the page text that has not been chosen before.
- If it is Decoder's turn, the chosen value $x$ is **added** to the message clarity.
- If it is Encoder's turn, the chosen value $x$ is **subtracted** from the message clarity.

The rules for choosing $x$ are:
1. On the very first move of the game, Decoder may choose **any** unselected word from the page text.
2. On every move after the first:
   - Let $m$ be the index of the word chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected word.

The game continues until all words of the page text have been chosen.

Decoder plays optimally to **maximize** the final message clarity, while Encoder plays optimally to **minimize** it.

Your task is to compute the final message clarity assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final message clarity is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final message clarity is 1.

## Input Format
- The first line contains an integer $n$ (length of page text).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final message clarity on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
