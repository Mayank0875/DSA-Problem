## Title
Encryption Key

## Slug
encryption-key

## Difficulty
Medium

## Description
A spy decrypts a message. The key is composed of Alpha ('A') and Beta ('B') waves.

The spy is working with a sequence represented by a string $s$ consisting of characters 'A' and 'B'.

To unlock the cypher, The spy must generate a **decryption key** $t$. A decryption key is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'A', then $t_i$ must be 'B'.
- If $s_i$ is 'B', then $t_i$ must be 'A'.

The decryption key $t$ is constructed by reusing the elements available in the original sequence $s$. The spy can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 wave.

Your goal is to construct the longest possible valid decryption key $t$ (starting from the beginning) using the available counts of 'A's and 'B's from $s$. Calculate the minimum waves required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
A

#### Output
1

#### Explanation
We have one 'A'. We need a 'B' to oppose $s[0]$. We have no 'B's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
ABB

#### Output
1

#### Explanation
Counts: 'A': 1, 'B': 2.
- Index 0 ($s[0]$='A'): Need 'B'. We have two 'B's. Use one. Remaining: 'A':1, 'B':1.
- Index 1 ($s[1]$='B'): Need 'A'. We have one 'A'. Use one. Remaining: 'A':0, 'B':1.
- Index 2 ($s[2]$='B'): Need 'A'. We have zero 'A's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'A' and 'B'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

