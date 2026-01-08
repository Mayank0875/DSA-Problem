## Title
Active Passive Voice

## Slug
active-passive-voice

## Difficulty
Medium

## Description
An editor fixes a manuscript. Sentences are Active ('A') or Passive ('P').

The editor is working with a sequence represented by a string $s$ consisting of characters 'A' and 'P'.

To improve readability, The editor must generate a **sentence flow** $t$. A sentence flow is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'A', then $t_i$ must be 'P'.
- If $s_i$ is 'P', then $t_i$ must be 'A'.

The sentence flow $t$ is constructed by reusing the elements available in the original sequence $s$. The editor can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 sentence.

Your goal is to construct the longest possible valid sentence flow $t$ (starting from the beginning) using the available counts of 'A's and 'P's from $s$. Calculate the minimum sentences required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
A

#### Output
1

#### Explanation
We have one 'A'. We need a 'P' to oppose $s[0]$. We have no 'P's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
APP

#### Output
1

#### Explanation
Counts: 'A': 1, 'P': 2.
- Index 0 ($s[0]$='A'): Need 'P'. We have two 'P's. Use one. Remaining: 'A':1, 'P':1.
- Index 1 ($s[1]$='P'): Need 'A'. We have one 'A'. Use one. Remaining: 'A':0, 'P':1.
- Index 2 ($s[2]$='P'): Need 'A'. We have zero 'A's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'A' and 'P'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

