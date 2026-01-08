## Title
Fast Slow Lane

## Slug
fast-slow-lane

## Difficulty
Medium

## Description
A traffic controller manages lanes. Cars are Fast ('F') or Slow ('S').

The controller is working with a sequence represented by a string $s$ consisting of characters 'F' and 'S'.

To prevent congestion, The controller must generate a **traffic flow** $t$. A traffic flow is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'F', then $t_i$ must be 'S'.
- If $s_i$ is 'S', then $t_i$ must be 'F'.

The traffic flow $t$ is constructed by reusing the elements available in the original sequence $s$. The controller can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 car.

Your goal is to construct the longest possible valid traffic flow $t$ (starting from the beginning) using the available counts of 'F's and 'S's from $s$. Calculate the minimum cars required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
F

#### Output
1

#### Explanation
We have one 'F'. We need a 'S' to oppose $s[0]$. We have no 'S's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
FSS

#### Output
1

#### Explanation
Counts: 'F': 1, 'S': 2.
- Index 0 ($s[0]$='F'): Need 'S'. We have two 'S's. Use one. Remaining: 'F':1, 'S':1.
- Index 1 ($s[1]$='S'): Need 'F'. We have one 'F'. Use one. Remaining: 'F':0, 'S':1.
- Index 2 ($s[2]$='S'): Need 'F'. We have zero 'F's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'F' and 'S'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

