## Title
Short Long Vowel

## Slug
short-long-vowel

## Difficulty
Medium

## Description
A linguist analyzes speech. Vowels are Short ('S') or Long ('L').

The linguist is working with a sequence represented by a string $s$ consisting of characters 'S' and 'L'.

To transcribe the accent, The linguist must generate a **pronunciation guide** $t$. A pronunciation guide is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'S', then $t_i$ must be 'L'.
- If $s_i$ is 'L', then $t_i$ must be 'S'.

The pronunciation guide $t$ is constructed by reusing the elements available in the original sequence $s$. The linguist can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 sound.

Your goal is to construct the longest possible valid pronunciation guide $t$ (starting from the beginning) using the available counts of 'S's and 'L's from $s$. Calculate the minimum sounds required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
S

#### Output
1

#### Explanation
We have one 'S'. We need a 'L' to oppose $s[0]$. We have no 'L's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
SLL

#### Output
1

#### Explanation
Counts: 'S': 1, 'L': 2.
- Index 0 ($s[0]$='S'): Need 'L'. We have two 'L's. Use one. Remaining: 'S':1, 'L':1.
- Index 1 ($s[1]$='L'): Need 'S'. We have one 'S'. Use one. Remaining: 'S':0, 'L':1.
- Index 2 ($s[2]$='L'): Need 'S'. We have zero 'S's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'S' and 'L'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

