## Title
Positive Negative Charge

## Slug
positive-negative-charge

## Difficulty
Medium

## Description
A battery system balances ions. The stream contains Positive ('+') and Negative ('-') charges.

The chemist is working with a sequence represented by a string $s$ consisting of characters '+' and '-'.

To neutralize the solution, The chemist must generate a **neutralizing flow** $t$. A neutralizing flow is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is '+', then $t_i$ must be '-'.
- If $s_i$ is '-', then $t_i$ must be '+'.

The neutralizing flow $t$ is constructed by reusing the elements available in the original sequence $s$. The chemist can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 charge.

Your goal is to construct the longest possible valid neutralizing flow $t$ (starting from the beginning) using the available counts of '+'s and '-'s from $s$. Calculate the minimum charges required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
+

#### Output
1

#### Explanation
We have one '+'. We need a '-' to oppose $s[0]$. We have no '-'s. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
+--

#### Output
1

#### Explanation
Counts: '+': 1, '-': 2.
- Index 0 ($s[0]$='+'): Need '-'. We have two '-'s. Use one. Remaining: '+':1, '-':1.
- Index 1 ($s[1]$='-'): Need '+'. We have one '+'. Use one. Remaining: '+':0, '-':1.
- Index 2 ($s[2]$='-'): Need '+'. We have zero '+'s. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters '+' and '-'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

