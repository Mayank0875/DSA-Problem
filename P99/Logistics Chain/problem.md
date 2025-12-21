## Title
Logistics Chain

## Slug
logistics-chain

## Difficulty
Hard

## Description
Truckers deliver cargo. Manifests list the next destination.

Trucker and Traffic are playing a strategic game using a route map $p$ of length $n$. The game starts with a delivery score of 0.

The players take turns, with Trucker moving first. On each turn, a player chooses an integer $x$ from the route map that has not been chosen before.
- If it is Trucker's turn, the chosen value $x$ is **added** to the delivery score.
- If it is Traffic's turn, the chosen value $x$ is **subtracted** from the delivery score.

The rules for choosing $x$ are:
1. On the very first move of the game, Trucker may choose **any** unselected stop from the route map.
2. On every move after the first:
   - Let $m$ be the index of the stop chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected stop.

The game continues until all stops of the route map have been chosen.

Trucker plays optimally to **maximize** the final delivery score, while Traffic plays optimally to **minimize** it.

Your task is to compute the final delivery score assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final delivery score is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final delivery score is 1.

## Input Format
- The first line contains an integer $n$ (length of route map).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final delivery score on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
