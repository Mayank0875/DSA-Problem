## Title
Light and Shadow

## Slug
light-and-shadow

## Difficulty
Medium

## Description
An artist is creating a high-contrast mosaic. The source image has Light ('L') and Dark ('D') tiles.

The artist is working with a sequence represented by a string $s$ consisting of characters 'L' and 'D'.

To balance the composition, The artist must generate a **contrast layer** $t$. A contrast layer is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'L', then $t_i$ must be 'D'.
- If $s_i$ is 'D', then $t_i$ must be 'L'.

The contrast layer $t$ is constructed by reusing the elements available in the original sequence $s$. The artist can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 tile.

Your goal is to construct the longest possible valid contrast layer $t$ (starting from the beginning) using the available counts of 'L's and 'D's from $s$. Calculate the minimum tiles required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
L

#### Output
1

#### Explanation
We have one 'L'. We need a 'D' to oppose $s[0]$. We have no 'D's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
LDD

#### Output
1

#### Explanation
Counts: 'L': 1, 'D': 2.
- Index 0 ($s[0]$='L'): Need 'D'. We have two 'D's. Use one. Remaining: 'L':1, 'D':1.
- Index 1 ($s[1]$='D'): Need 'L'. We have one 'L'. Use one. Remaining: 'L':0, 'D':1.
- Index 2 ($s[2]$='D'): Need 'L'. We have zero 'L's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'L' and 'D'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

