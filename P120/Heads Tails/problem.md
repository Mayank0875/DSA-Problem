## Title
Heads Tails

## Slug
heads-tails

## Difficulty
Medium

## Description
A statistician flips coins. Outcomes are Heads ('H') or Tails ('T').

The statistician is working with a sequence represented by a string $s$ consisting of characters 'H' and 'T'.

To prove probability, The statistician must generate a **fair coin check** $t$. A fair coin check is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'H', then $t_i$ must be 'T'.
- If $s_i$ is 'T', then $t_i$ must be 'H'.

The fair coin check $t$ is constructed by reusing the elements available in the original sequence $s$. The statistician can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 flip.

Your goal is to construct the longest possible valid fair coin check $t$ (starting from the beginning) using the available counts of 'H's and 'T's from $s$. Calculate the minimum flips required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
H

#### Output
1

#### Explanation
We have one 'H'. We need a 'T' to oppose $s[0]$. We have no 'T's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
HTT

#### Output
1

#### Explanation
Counts: 'H': 1, 'T': 2.
- Index 0 ($s[0]$='H'): Need 'T'. We have two 'T's. Use one. Remaining: 'H':1, 'T':1.
- Index 1 ($s[1]$='T'): Need 'H'. We have one 'H'. Use one. Remaining: 'H':0, 'T':1.
- Index 2 ($s[2]$='T'): Need 'H'. We have zero 'H's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'H' and 'T'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

