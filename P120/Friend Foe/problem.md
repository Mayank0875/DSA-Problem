## Title
Friend Foe

## Slug
friend-foe

## Difficulty
Medium

## Description
A radar operator identifies blips. Targets are Friend ('F') or Foe ('E').

The operator is working with a sequence represented by a string $s$ consisting of characters 'F' and 'E'.

To secure the airspace, The operator must generate a **IFF response** $t$. A IFF response is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'F', then $t_i$ must be 'E'.
- If $s_i$ is 'E', then $t_i$ must be 'F'.

The IFF response $t$ is constructed by reusing the elements available in the original sequence $s$. The operator can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 blip.

Your goal is to construct the longest possible valid IFF response $t$ (starting from the beginning) using the available counts of 'F's and 'E's from $s$. Calculate the minimum blips required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
F

#### Output
1

#### Explanation
We have one 'F'. We need a 'E' to oppose $s[0]$. We have no 'E's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
FEE

#### Output
1

#### Explanation
Counts: 'F': 1, 'E': 2.
- Index 0 ($s[0]$='F'): Need 'E'. We have two 'E's. Use one. Remaining: 'F':1, 'E':1.
- Index 1 ($s[1]$='E'): Need 'F'. We have one 'F'. Use one. Remaining: 'F':0, 'E':1.
- Index 2 ($s[2]$='E'): Need 'F'. We have zero 'F's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'F' and 'E'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

