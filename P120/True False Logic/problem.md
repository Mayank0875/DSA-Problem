## Title
True False Logic

## Slug
true-false-logic

## Difficulty
Medium

## Description
A philosopher debates. Arguments are premises of True ('T') or False ('F').

The philosopher is working with a sequence represented by a string $s$ consisting of characters 'T' and 'F'.

To construct a paradox, The philosopher must generate a **negation chain** $t$. A negation chain is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'T', then $t_i$ must be 'F'.
- If $s_i$ is 'F', then $t_i$ must be 'T'.

The negation chain $t$ is constructed by reusing the elements available in the original sequence $s$. The philosopher can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 proposition.

Your goal is to construct the longest possible valid negation chain $t$ (starting from the beginning) using the available counts of 'T's and 'F's from $s$. Calculate the minimum propositions required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
T

#### Output
1

#### Explanation
We have one 'T'. We need a 'F' to oppose $s[0]$. We have no 'F's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
TFF

#### Output
1

#### Explanation
Counts: 'T': 1, 'F': 2.
- Index 0 ($s[0]$='T'): Need 'F'. We have two 'F's. Use one. Remaining: 'T':1, 'F':1.
- Index 1 ($s[1]$='F'): Need 'T'. We have one 'T'. Use one. Remaining: 'T':0, 'F':1.
- Index 2 ($s[2]$='F'): Need 'T'. We have zero 'T's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'T' and 'F'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

