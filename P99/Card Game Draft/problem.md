## Title
Card Game Draft

## Slug
card-game-draft

## Difficulty
Hard

## Description
Players draft cards. Each card has a 'combo' pointer to another card.

Player 1 and Player 2 are playing a strategic game using a deck order $p$ of length $n$. The game starts with a deck strength of 0.

The players take turns, with Player 1 moving first. On each turn, a player chooses an integer $x$ from the deck order that has not been chosen before.
- If it is Player 1's turn, the chosen value $x$ is **added** to the deck strength.
- If it is Player 2's turn, the chosen value $x$ is **subtracted** from the deck strength.

The rules for choosing $x$ are:
1. On the very first move of the game, Player 1 may choose **any** unselected card from the deck order.
2. On every move after the first:
   - Let $m$ be the index of the card chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected card.

The game continues until all cards of the deck order have been chosen.

Player 1 plays optimally to **maximize** the final deck strength, while Player 2 plays optimally to **minimize** it.

Your task is to compute the final deck strength assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final deck strength is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final deck strength is 1.

## Input Format
- The first line contains an integer $n$ (length of deck order).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final deck strength on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
