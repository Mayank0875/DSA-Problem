## Title
Question Answer

## Slug
question-answer

## Difficulty
Medium

## Description
A teacher grades a quiz. Lines are Questions ('Q') or Answers ('A').

The teacher is working with a sequence represented by a string $s$ consisting of characters 'Q' and 'A'.

To grade the paper, The teacher must generate a **Q&A pair** $t$. A Q&A pair is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'Q', then $t_i$ must be 'A'.
- If $s_i$ is 'A', then $t_i$ must be 'Q'.

The Q&A pair $t$ is constructed by reusing the elements available in the original sequence $s$. The teacher can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 line.

Your goal is to construct the longest possible valid Q&A pair $t$ (starting from the beginning) using the available counts of 'Q's and 'A's from $s$. Calculate the minimum lines required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
Q

#### Output
1

#### Explanation
We have one 'Q'. We need a 'A' to oppose $s[0]$. We have no 'A's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
QAA

#### Output
1

#### Explanation
Counts: 'Q': 1, 'A': 2.
- Index 0 ($s[0]$='Q'): Need 'A'. We have two 'A's. Use one. Remaining: 'Q':1, 'A':1.
- Index 1 ($s[1]$='A'): Need 'Q'. We have one 'Q'. Use one. Remaining: 'Q':0, 'A':1.
- Index 2 ($s[2]$='A'): Need 'Q'. We have zero 'Q's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'Q' and 'A'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

