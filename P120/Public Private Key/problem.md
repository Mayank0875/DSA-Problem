## Title
Public Private Key

## Slug
public-private-key

## Difficulty
Medium

## Description
A cryptographer generates keys. Parts are Public ('P') or Private ('V').

The cryptographer is working with a sequence represented by a string $s$ consisting of characters 'P' and 'V'.

To secure the channel, The cryptographer must generate a **key pair** $t$. A key pair is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'P', then $t_i$ must be 'V'.
- If $s_i$ is 'V', then $t_i$ must be 'P'.

The key pair $t$ is constructed by reusing the elements available in the original sequence $s$. The cryptographer can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 part.

Your goal is to construct the longest possible valid key pair $t$ (starting from the beginning) using the available counts of 'P's and 'V's from $s$. Calculate the minimum parts required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
P

#### Output
1

#### Explanation
We have one 'P'. We need a 'V' to oppose $s[0]$. We have no 'V's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
PVV

#### Output
1

#### Explanation
Counts: 'P': 1, 'V': 2.
- Index 0 ($s[0]$='P'): Need 'V'. We have two 'V's. Use one. Remaining: 'P':1, 'V':1.
- Index 1 ($s[1]$='V'): Need 'P'. We have one 'P'. Use one. Remaining: 'P':0, 'V':1.
- Index 2 ($s[2]$='V'): Need 'P'. We have zero 'P's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'P' and 'V'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

