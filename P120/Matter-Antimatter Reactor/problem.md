## Title
Matter-Antimatter Reactor

## Slug
matter-antimatter-reactor

## Difficulty
Medium

## Description
A physicist is feeding a reactor. The fuel stream has Matter ('M') and Antimatter ('A') particles.

Dr. Stone is working with a sequence represented by a string $s$ consisting of characters 'M' and 'A'.

To prevent an explosion, Dr. Stone must generate a **containment stream** $t$. A containment stream is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'M', then $t_i$ must be 'A'.
- If $s_i$ is 'A', then $t_i$ must be 'M'.

The containment stream $t$ is constructed by reusing the elements available in the original sequence $s$. Dr. Stone can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 particle.

Your goal is to construct the longest possible valid containment stream $t$ (starting from the beginning) using the available counts of 'M's and 'A's from $s$. Calculate the minimum particles required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
M

#### Output
1

#### Explanation
We have one 'M'. We need a 'A' to oppose $s[0]$. We have no 'A's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
MAA

#### Output
1

#### Explanation
Counts: 'M': 1, 'A': 2.
- Index 0 ($s[0]$='M'): Need 'A'. We have two 'A's. Use one. Remaining: 'M':1, 'A':1.
- Index 1 ($s[1]$='A'): Need 'M'. We have one 'M'. Use one. Remaining: 'M':0, 'A':1.
- Index 2 ($s[2]$='A'): Need 'M'. We have zero 'M's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'M' and 'A'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

