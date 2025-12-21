## Title
Stock Market Duel

## Slug
stock-market-duel

## Difficulty
Hard

## Description
Two traders compete to acquire stocks in a linked portfolio.

Bull and Bear are playing a strategic game using a stock listing $p$ of length $n$. The game starts with a profit margin of 0.

The players take turns, with Bull moving first. On each turn, a player chooses an integer $x$ from the stock listing that has not been chosen before.
- If it is Bull's turn, the chosen value $x$ is **added** to the profit margin.
- If it is Bear's turn, the chosen value $x$ is **subtracted** from the profit margin.

The rules for choosing $x$ are:
1. On the very first move of the game, Bull may choose **any** unselected stock from the stock listing.
2. On every move after the first:
   - Let $m$ be the index of the stock chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected stock.

The game continues until all stocks of the stock listing have been chosen.

Bull plays optimally to **maximize** the final profit margin, while Bear plays optimally to **minimize** it.

Your task is to compute the final profit margin assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final profit margin is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final profit margin is 1.

## Input Format
- The first line contains an integer $n$ (length of stock listing).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final profit margin on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
