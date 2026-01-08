## Title
Sun and Moon

## Slug
sun-and-moon

## Difficulty
Medium

## Description
A celestial temple aligns totems. The totems represent Sun ('S') and Moon ('M').

The priest is working with a sequence represented by a string $s$ consisting of characters 'S' and 'M'.

To maintain cosmic balance, The priest must generate a **eclipse alignment** $t$. A eclipse alignment is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'S', then $t_i$ must be 'M'.
- If $s_i$ is 'M', then $t_i$ must be 'S'.

The eclipse alignment $t$ is constructed by reusing the elements available in the original sequence $s$. The priest can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 totem.

Your goal is to construct the longest possible valid eclipse alignment $t$ (starting from the beginning) using the available counts of 'S's and 'M's from $s$. Calculate the minimum totems required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
S

#### Output
1

#### Explanation
We have one 'S'. We need a 'M' to oppose $s[0]$. We have no 'M's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
SMM

#### Output
1

#### Explanation
Counts: 'S': 1, 'M': 2.
- Index 0 ($s[0]$='S'): Need 'M'. We have two 'M's. Use one. Remaining: 'S':1, 'M':1.
- Index 1 ($s[1]$='M'): Need 'S'. We have one 'S'. Use one. Remaining: 'S':0, 'M':1.
- Index 2 ($s[2]$='M'): Need 'S'. We have zero 'S's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'S' and 'M'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

