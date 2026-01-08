## Title
Debit Credit

## Slug
debit-credit

## Difficulty
Medium

## Description
An accountant balances the books. Entries are Debit ('D') or Credit ('C').

The accountant is working with a sequence represented by a string $s$ consisting of characters 'D' and 'C'.

To zero out the ledger, The accountant must generate a **balanced sheet** $t$. A balanced sheet is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'D', then $t_i$ must be 'C'.
- If $s_i$ is 'C', then $t_i$ must be 'D'.

The balanced sheet $t$ is constructed by reusing the elements available in the original sequence $s$. The accountant can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 entry.

Your goal is to construct the longest possible valid balanced sheet $t$ (starting from the beginning) using the available counts of 'D's and 'C's from $s$. Calculate the minimum entrys required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
D

#### Output
1

#### Explanation
We have one 'D'. We need a 'C' to oppose $s[0]$. We have no 'C's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
DCC

#### Output
1

#### Explanation
Counts: 'D': 1, 'C': 2.
- Index 0 ($s[0]$='D'): Need 'C'. We have two 'C's. Use one. Remaining: 'D':1, 'C':1.
- Index 1 ($s[1]$='C'): Need 'D'. We have one 'D'. Use one. Remaining: 'D':0, 'C':1.
- Index 2 ($s[2]$='C'): Need 'D'. We have zero 'D's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'D' and 'C'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

