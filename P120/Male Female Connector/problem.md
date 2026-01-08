## Title
Male Female Connector

## Slug
male-female-connector

## Difficulty
Medium

## Description
A plumber fits pipes. Connectors are Male ('M') or Female ('F').

The plumber is working with a sequence represented by a string $s$ consisting of characters 'M' and 'F'.

To extend the pipeline, The plumber must generate a **pipe fitting** $t$. A pipe fitting is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'M', then $t_i$ must be 'F'.
- If $s_i$ is 'F', then $t_i$ must be 'M'.

The pipe fitting $t$ is constructed by reusing the elements available in the original sequence $s$. The plumber can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 connector.

Your goal is to construct the longest possible valid pipe fitting $t$ (starting from the beginning) using the available counts of 'M's and 'F's from $s$. Calculate the minimum connectors required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
M

#### Output
1

#### Explanation
We have one 'M'. We need a 'F' to oppose $s[0]$. We have no 'F's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
MFF

#### Output
1

#### Explanation
Counts: 'M': 1, 'F': 2.
- Index 0 ($s[0]$='M'): Need 'F'. We have two 'F's. Use one. Remaining: 'M':1, 'F':1.
- Index 1 ($s[1]$='F'): Need 'M'. We have one 'M'. Use one. Remaining: 'M':0, 'F':1.
- Index 2 ($s[2]$='F'): Need 'M'. We have zero 'M's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'M' and 'F'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

