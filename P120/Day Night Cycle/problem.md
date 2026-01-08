## Title
Day Night Cycle

## Slug
day-night-cycle

## Difficulty
Medium

## Description
A simulator runs a world. The timeline consists of Day ('D') and Night ('N') phases.

The admin is working with a sequence represented by a string $s$ consisting of characters 'D' and 'N'.

To ensure circadian rhythm, The admin must generate a **sleep schedule** $t$. A sleep schedule is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'D', then $t_i$ must be 'N'.
- If $s_i$ is 'N', then $t_i$ must be 'D'.

The sleep schedule $t$ is constructed by reusing the elements available in the original sequence $s$. The admin can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 hour.

Your goal is to construct the longest possible valid sleep schedule $t$ (starting from the beginning) using the available counts of 'D's and 'N's from $s$. Calculate the minimum hours required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
D

#### Output
1

#### Explanation
We have one 'D'. We need a 'N' to oppose $s[0]$. We have no 'N's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
DNN

#### Output
1

#### Explanation
Counts: 'D': 1, 'N': 2.
- Index 0 ($s[0]$='D'): Need 'N'. We have two 'N's. Use one. Remaining: 'D':1, 'N':1.
- Index 1 ($s[1]$='N'): Need 'D'. We have one 'D'. Use one. Remaining: 'D':0, 'N':1.
- Index 2 ($s[2]$='N'): Need 'D'. We have zero 'D's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'D' and 'N'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

