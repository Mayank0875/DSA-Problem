## Title
Auction Bidding

## Slug
auction-bidding

## Difficulty
Hard

## Description
Collectors bid on lots. Winning a lot gives priority for a specific next lot.

Bidder A and Bidder B are playing a strategic game using a lot list $p$ of length $n$. The game starts with a collection value of 0.

The players take turns, with Bidder A moving first. On each turn, a player chooses an integer $x$ from the lot list that has not been chosen before.
- If it is Bidder A's turn, the chosen value $x$ is **added** to the collection value.
- If it is Bidder B's turn, the chosen value $x$ is **subtracted** from the collection value.

The rules for choosing $x$ are:
1. On the very first move of the game, Bidder A may choose **any** unselected lot from the lot list.
2. On every move after the first:
   - Let $m$ be the index of the lot chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected lot.

The game continues until all lots of the lot list have been chosen.

Bidder A plays optimally to **maximize** the final collection value, while Bidder B plays optimally to **minimize** it.

Your task is to compute the final collection value assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final collection value is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final collection value is 1.

## Input Format
- The first line contains an integer $n$ (length of lot list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final collection value on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
