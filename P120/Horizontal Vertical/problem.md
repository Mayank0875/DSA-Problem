## Title
Horizontal Vertical

## Slug
horizontal-vertical

## Difficulty
Medium

## Description
A weaver sets a loom. Threads are Horizontal ('H') or Vertical ('V').

The weaver is working with a sequence represented by a string $s$ consisting of characters 'H' and 'V'.

To weave the fabric, The weaver must generate a **cross-stitch** $t$. A cross-stitch is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'H', then $t_i$ must be 'V'.
- If $s_i$ is 'V', then $t_i$ must be 'H'.

The cross-stitch $t$ is constructed by reusing the elements available in the original sequence $s$. The weaver can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 thread.

Your goal is to construct the longest possible valid cross-stitch $t$ (starting from the beginning) using the available counts of 'H's and 'V's from $s$. Calculate the minimum threads required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
H

#### Output
1

#### Explanation
We have one 'H'. We need a 'V' to oppose $s[0]$. We have no 'V's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
HVV

#### Output
1

#### Explanation
Counts: 'H': 1, 'V': 2.
- Index 0 ($s[0]$='H'): Need 'V'. We have two 'V's. Use one. Remaining: 'H':1, 'V':1.
- Index 1 ($s[1]$='V'): Need 'H'. We have one 'H'. Use one. Remaining: 'H':0, 'V':1.
- Index 2 ($s[2]$='V'): Need 'H'. We have zero 'H's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'H' and 'V'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

