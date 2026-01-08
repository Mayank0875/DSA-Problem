## Title
Magnetic Shield

## Slug
magnetic-shield

## Difficulty
Medium

## Description
An engineer needs to neutralize a magnetic field. The field consists of North ('N') and South ('S') poles.

The engineer is working with a sequence represented by a string $s$ consisting of characters 'N' and 'S'.

To create a zero-net-flux shield, The engineer must generate a **anti-field** $t$. A anti-field is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'N', then $t_i$ must be 'S'.
- If $s_i$ is 'S', then $t_i$ must be 'N'.

The anti-field $t$ is constructed by reusing the elements available in the original sequence $s$. The engineer can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 energy unit.

Your goal is to construct the longest possible valid anti-field $t$ (starting from the beginning) using the available counts of 'N's and 'S's from $s$. Calculate the minimum energy units required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
N

#### Output
1

#### Explanation
We have one 'N'. We need a 'S' to oppose $s[0]$. We have no 'S's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
NSS

#### Output
1

#### Explanation
Counts: 'N': 1, 'S': 2.
- Index 0 ($s[0]$='N'): Need 'S'. We have two 'S's. Use one. Remaining: 'N':1, 'S':1.
- Index 1 ($s[1]$='S'): Need 'N'. We have one 'N'. Use one. Remaining: 'N':0, 'S':1.
- Index 2 ($s[2]$='S'): Need 'N'. We have zero 'N's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'N' and 'S'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

