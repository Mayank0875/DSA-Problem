## Title
Dry Wet Season

## Slug
dry-wet-season

## Difficulty
Medium

## Description
A climatologist studies history. Years are Dry ('D') or Wet ('W').

The scientist is working with a sequence represented by a string $s$ consisting of characters 'D' and 'W'.

To model the climate, The scientist must generate a **weather cycle** $t$. A weather cycle is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'D', then $t_i$ must be 'W'.
- If $s_i$ is 'W', then $t_i$ must be 'D'.

The weather cycle $t$ is constructed by reusing the elements available in the original sequence $s$. The scientist can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 year.

Your goal is to construct the longest possible valid weather cycle $t$ (starting from the beginning) using the available counts of 'D's and 'W's from $s$. Calculate the minimum years required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
D

#### Output
1

#### Explanation
We have one 'D'. We need a 'W' to oppose $s[0]$. We have no 'W's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
DWW

#### Output
1

#### Explanation
Counts: 'D': 1, 'W': 2.
- Index 0 ($s[0]$='D'): Need 'W'. We have two 'W's. Use one. Remaining: 'D':1, 'W':1.
- Index 1 ($s[1]$='W'): Need 'D'. We have one 'D'. Use one. Remaining: 'D':0, 'W':1.
- Index 2 ($s[2]$='W'): Need 'D'. We have zero 'D's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'D' and 'W'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

