## Title
Alpha Omega

## Slug
alpha-omega

## Difficulty
Medium

## Description
A theologian studies a text. Symbols are Alpha ('A') and Omega ('O').

The scholar is working with a sequence represented by a string $s$ consisting of characters 'A' and 'O'.

To find the beginning and end, The scholar must generate a **complete cycle** $t$. A complete cycle is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'A', then $t_i$ must be 'O'.
- If $s_i$ is 'O', then $t_i$ must be 'A'.

The complete cycle $t$ is constructed by reusing the elements available in the original sequence $s$. The scholar can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 symbol.

Your goal is to construct the longest possible valid complete cycle $t$ (starting from the beginning) using the available counts of 'A's and 'O's from $s$. Calculate the minimum symbols required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
A

#### Output
1

#### Explanation
We have one 'A'. We need a 'O' to oppose $s[0]$. We have no 'O's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
AOO

#### Output
1

#### Explanation
Counts: 'A': 1, 'O': 2.
- Index 0 ($s[0]$='A'): Need 'O'. We have two 'O's. Use one. Remaining: 'A':1, 'O':1.
- Index 1 ($s[1]$='O'): Need 'A'. We have one 'A'. Use one. Remaining: 'A':0, 'O':1.
- Index 2 ($s[2]$='O'): Need 'A'. We have zero 'A's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'A' and 'O'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

