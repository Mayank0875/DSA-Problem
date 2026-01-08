## Title
Wax Wane Moon

## Slug
wax-wane-moon

## Difficulty
Medium

## Description
An astrologer tracks the moon. Phases are Waxing ('W') or Waning ('N').

The astrologer is working with a sequence represented by a string $s$ consisting of characters 'W' and 'N'.

To predict the tide, The astrologer must generate a **lunar cycle** $t$. A lunar cycle is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'W', then $t_i$ must be 'N'.
- If $s_i$ is 'N', then $t_i$ must be 'W'.

The lunar cycle $t$ is constructed by reusing the elements available in the original sequence $s$. The astrologer can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 phase.

Your goal is to construct the longest possible valid lunar cycle $t$ (starting from the beginning) using the available counts of 'W's and 'N's from $s$. Calculate the minimum phases required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
W

#### Output
1

#### Explanation
We have one 'W'. We need a 'N' to oppose $s[0]$. We have no 'N's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
WNN

#### Output
1

#### Explanation
Counts: 'W': 1, 'N': 2.
- Index 0 ($s[0]$='W'): Need 'N'. We have two 'N's. Use one. Remaining: 'W':1, 'N':1.
- Index 1 ($s[1]$='N'): Need 'W'. We have one 'W'. Use one. Remaining: 'W':0, 'N':1.
- Index 2 ($s[2]$='N'): Need 'W'. We have zero 'W's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'W' and 'N'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

