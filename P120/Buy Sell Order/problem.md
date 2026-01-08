## Title
Buy Sell Order

## Slug
buy-sell-order

## Difficulty
Medium

## Description
A stock bot executes trades. Orders are Buy ('B') or Sell ('S').

The bot is working with a sequence represented by a string $s$ consisting of characters 'B' and 'S'.

To close all positions, The bot must generate a **market neutral strategy** $t$. A market neutral strategy is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'B', then $t_i$ must be 'S'.
- If $s_i$ is 'S', then $t_i$ must be 'B'.

The market neutral strategy $t$ is constructed by reusing the elements available in the original sequence $s$. The bot can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 order.

Your goal is to construct the longest possible valid market neutral strategy $t$ (starting from the beginning) using the available counts of 'B's and 'S's from $s$. Calculate the minimum orders required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
B

#### Output
1

#### Explanation
We have one 'B'. We need a 'S' to oppose $s[0]$. We have no 'S's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
BSS

#### Output
1

#### Explanation
Counts: 'B': 1, 'S': 2.
- Index 0 ($s[0]$='B'): Need 'S'. We have two 'S's. Use one. Remaining: 'B':1, 'S':1.
- Index 1 ($s[1]$='S'): Need 'B'. We have one 'B'. Use one. Remaining: 'B':0, 'S':1.
- Index 2 ($s[2]$='S'): Need 'B'. We have zero 'B's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'B' and 'S'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

