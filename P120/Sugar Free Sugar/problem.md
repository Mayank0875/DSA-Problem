## Title
Sugar Free Sugar

## Slug
sugar-free-sugar

## Difficulty
Medium

## Description
A barista makes drinks. Requests are Sugar ('S') or Zero ('Z').

The barista is working with a sequence represented by a string $s$ consisting of characters 'S' and 'Z'.

To serve the line, The barista must generate a **drink order** $t$. A drink order is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'S', then $t_i$ must be 'Z'.
- If $s_i$ is 'Z', then $t_i$ must be 'S'.

The drink order $t$ is constructed by reusing the elements available in the original sequence $s$. The barista can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 packet.

Your goal is to construct the longest possible valid drink order $t$ (starting from the beginning) using the available counts of 'S's and 'Z's from $s$. Calculate the minimum packets required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
S

#### Output
1

#### Explanation
We have one 'S'. We need a 'Z' to oppose $s[0]$. We have no 'Z's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
SZZ

#### Output
1

#### Explanation
Counts: 'S': 1, 'Z': 2.
- Index 0 ($s[0]$='S'): Need 'Z'. We have two 'Z's. Use one. Remaining: 'S':1, 'Z':1.
- Index 1 ($s[1]$='Z'): Need 'S'. We have one 'S'. Use one. Remaining: 'S':0, 'Z':1.
- Index 2 ($s[2]$='Z'): Need 'S'. We have zero 'S's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'S' and 'Z'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

