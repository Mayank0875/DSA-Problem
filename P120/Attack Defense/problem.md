## Title
Attack Defense

## Slug
attack-defense

## Difficulty
Medium

## Description
A strategy game AI plans moves. Moves are Attack ('A') or Defend ('D').

The AI is working with a sequence represented by a string $s$ consisting of characters 'A' and 'D'.

To counter the opponent, The AI must generate a **perfect counter-play** $t$. A perfect counter-play is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'A', then $t_i$ must be 'D'.
- If $s_i$ is 'D', then $t_i$ must be 'A'.

The perfect counter-play $t$ is constructed by reusing the elements available in the original sequence $s$. The AI can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 move.

Your goal is to construct the longest possible valid perfect counter-play $t$ (starting from the beginning) using the available counts of 'A's and 'D's from $s$. Calculate the minimum moves required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
A

#### Output
1

#### Explanation
We have one 'A'. We need a 'D' to oppose $s[0]$. We have no 'D's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
ADD

#### Output
1

#### Explanation
Counts: 'A': 1, 'D': 2.
- Index 0 ($s[0]$='A'): Need 'D'. We have two 'D's. Use one. Remaining: 'A':1, 'D':1.
- Index 1 ($s[1]$='D'): Need 'A'. We have one 'A'. Use one. Remaining: 'A':0, 'D':1.
- Index 2 ($s[2]$='D'): Need 'A'. We have zero 'A's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'A' and 'D'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

