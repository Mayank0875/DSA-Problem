## Title
Proton Electron

## Slug
proton-electron

## Difficulty
Medium

## Description
A physics simulation tracks particles. Protons ('P') and Electrons ('E') are in a cloud.

The physicist is working with a sequence represented by a string $s$ consisting of characters 'P' and 'E'.

To form hydrogen atoms, The physicist must generate a **atomic assembly** $t$. A atomic assembly is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'P', then $t_i$ must be 'E'.
- If $s_i$ is 'E', then $t_i$ must be 'P'.

The atomic assembly $t$ is constructed by reusing the elements available in the original sequence $s$. The physicist can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 particle.

Your goal is to construct the longest possible valid atomic assembly $t$ (starting from the beginning) using the available counts of 'P's and 'E's from $s$. Calculate the minimum particles required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
P

#### Output
1

#### Explanation
We have one 'P'. We need a 'E' to oppose $s[0]$. We have no 'E's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
PEE

#### Output
1

#### Explanation
Counts: 'P': 1, 'E': 2.
- Index 0 ($s[0]$='P'): Need 'E'. We have two 'E's. Use one. Remaining: 'P':1, 'E':1.
- Index 1 ($s[1]$='E'): Need 'P'. We have one 'P'. Use one. Remaining: 'P':0, 'E':1.
- Index 2 ($s[2]$='E'): Need 'P'. We have zero 'P's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'P' and 'E'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

