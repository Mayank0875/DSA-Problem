## Title
Top Bottom Quark

## Slug
top-bottom-quark

## Difficulty
Medium

## Description
Another particle experiment. This time with Top ('T') and Bottom ('B') quarks.

The scientist is working with a sequence represented by a string $s$ consisting of characters 'T' and 'B'.

To maintain stability, The scientist must generate a **quark pair** $t$. A quark pair is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'T', then $t_i$ must be 'B'.
- If $s_i$ is 'B', then $t_i$ must be 'T'.

The quark pair $t$ is constructed by reusing the elements available in the original sequence $s$. The scientist can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 quark.

Your goal is to construct the longest possible valid quark pair $t$ (starting from the beginning) using the available counts of 'T's and 'B's from $s$. Calculate the minimum quarks required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
T

#### Output
1

#### Explanation
We have one 'T'. We need a 'B' to oppose $s[0]$. We have no 'B's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
TBB

#### Output
1

#### Explanation
Counts: 'T': 1, 'B': 2.
- Index 0 ($s[0]$='T'): Need 'B'. We have two 'B's. Use one. Remaining: 'T':1, 'B':1.
- Index 1 ($s[1]$='B'): Need 'T'. We have one 'T'. Use one. Remaining: 'T':0, 'B':1.
- Index 2 ($s[2]$='B'): Need 'T'. We have zero 'T's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'T' and 'B'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

