## Title
Odd Even Parity

## Slug
odd-even-parity

## Difficulty
Medium

## Description
A network engineer checks parity bits. Bits are Odd ('O') or Even ('E').

The engineer is working with a sequence represented by a string $s$ consisting of characters 'O' and 'E'.

To error correction, The engineer must generate a **parity check** $t$. A parity check is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'O', then $t_i$ must be 'E'.
- If $s_i$ is 'E', then $t_i$ must be 'O'.

The parity check $t$ is constructed by reusing the elements available in the original sequence $s$. The engineer can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 bit.

Your goal is to construct the longest possible valid parity check $t$ (starting from the beginning) using the available counts of 'O's and 'E's from $s$. Calculate the minimum bits required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
O

#### Output
1

#### Explanation
We have one 'O'. We need a 'E' to oppose $s[0]$. We have no 'E's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
OEE

#### Output
1

#### Explanation
Counts: 'O': 1, 'E': 2.
- Index 0 ($s[0]$='O'): Need 'E'. We have two 'E's. Use one. Remaining: 'O':1, 'E':1.
- Index 1 ($s[1]$='E'): Need 'O'. We have one 'O'. Use one. Remaining: 'O':0, 'E':1.
- Index 2 ($s[2]$='E'): Need 'O'. We have zero 'O's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'O' and 'E'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

