## Title
Land Sea Map

## Slug
land-sea-map

## Difficulty
Medium

## Description
A cartographer draws a coast. Tiles are Land ('L') or Sea ('S').

The cartographer is working with a sequence represented by a string $s$ consisting of characters 'L' and 'S'.

To define the coastline, The cartographer must generate a **boundary line** $t$. A boundary line is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'L', then $t_i$ must be 'S'.
- If $s_i$ is 'S', then $t_i$ must be 'L'.

The boundary line $t$ is constructed by reusing the elements available in the original sequence $s$. The cartographer can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 tile.

Your goal is to construct the longest possible valid boundary line $t$ (starting from the beginning) using the available counts of 'L's and 'S's from $s$. Calculate the minimum tiles required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
L

#### Output
1

#### Explanation
We have one 'L'. We need a 'S' to oppose $s[0]$. We have no 'S's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
LSS

#### Output
1

#### Explanation
Counts: 'L': 1, 'S': 2.
- Index 0 ($s[0]$='L'): Need 'S'. We have two 'S's. Use one. Remaining: 'L':1, 'S':1.
- Index 1 ($s[1]$='S'): Need 'L'. We have one 'L'. Use one. Remaining: 'L':0, 'S':1.
- Index 2 ($s[2]$='S'): Need 'L'. We have zero 'L's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'L' and 'S'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

