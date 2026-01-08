## Title
Import Export

## Slug
import-export

## Difficulty
Medium

## Description
A logistics manager tracks containers. Goods are Import ('I') or Export ('E').

The manager is working with a sequence represented by a string $s$ consisting of characters 'I' and 'E'.

To balance trade, The manager must generate a **shipping manifest** $t$. A shipping manifest is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'I', then $t_i$ must be 'E'.
- If $s_i$ is 'E', then $t_i$ must be 'I'.

The shipping manifest $t$ is constructed by reusing the elements available in the original sequence $s$. The manager can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 container.

Your goal is to construct the longest possible valid shipping manifest $t$ (starting from the beginning) using the available counts of 'I's and 'E's from $s$. Calculate the minimum containers required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
I

#### Output
1

#### Explanation
We have one 'I'. We need a 'E' to oppose $s[0]$. We have no 'E's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
IEE

#### Output
1

#### Explanation
Counts: 'I': 1, 'E': 2.
- Index 0 ($s[0]$='I'): Need 'E'. We have two 'E's. Use one. Remaining: 'I':1, 'E':1.
- Index 1 ($s[1]$='E'): Need 'I'. We have one 'I'. Use one. Remaining: 'I':0, 'E':1.
- Index 2 ($s[2]$='E'): Need 'I'. We have zero 'I's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'I' and 'E'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

