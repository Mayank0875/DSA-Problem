## Title
High Low Voltage

## Slug
high-low-voltage

## Difficulty
Medium

## Description
An electrician fixes a signal. The wire carries High ('H') and Low ('L') voltage pulses.

The electrician is working with a sequence represented by a string $s$ consisting of characters 'H' and 'L'.

To stabilize the transformer, The electrician must generate a **grounding sequence** $t$. A grounding sequence is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'H', then $t_i$ must be 'L'.
- If $s_i$ is 'L', then $t_i$ must be 'H'.

The grounding sequence $t$ is constructed by reusing the elements available in the original sequence $s$. The electrician can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 pulse.

Your goal is to construct the longest possible valid grounding sequence $t$ (starting from the beginning) using the available counts of 'H's and 'L's from $s$. Calculate the minimum pulses required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
H

#### Output
1

#### Explanation
We have one 'H'. We need a 'L' to oppose $s[0]$. We have no 'L's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
HLL

#### Output
1

#### Explanation
Counts: 'H': 1, 'L': 2.
- Index 0 ($s[0]$='H'): Need 'L'. We have two 'L's. Use one. Remaining: 'H':1, 'L':1.
- Index 1 ($s[1]$='L'): Need 'H'. We have one 'H'. Use one. Remaining: 'H':0, 'L':1.
- Index 2 ($s[2]$='L'): Need 'H'. We have zero 'H's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'H' and 'L'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

