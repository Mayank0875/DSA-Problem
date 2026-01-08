## Title
Acid Base Titration

## Slug
acid-base-titration

## Difficulty
Medium

## Description
A lab experiment mixes solutions. Drops are either Acidic ('A') or Basic ('B').

The student is working with a sequence represented by a string $s$ consisting of characters 'A' and 'B'.

To neutralize the pH, The student must generate a **buffer solution** $t$. A buffer solution is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'A', then $t_i$ must be 'B'.
- If $s_i$ is 'B', then $t_i$ must be 'A'.

The buffer solution $t$ is constructed by reusing the elements available in the original sequence $s$. The student can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 drop.

Your goal is to construct the longest possible valid buffer solution $t$ (starting from the beginning) using the available counts of 'A's and 'B's from $s$. Calculate the minimum drops required, which equals the number of elements discarded from $s$.

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

