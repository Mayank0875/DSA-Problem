## Title
Heating Cooling

## Slug
heating-cooling

## Difficulty
Medium

## Description
A thermostat regulates temp. Cycles are Heating ('H') or Cooling ('C').

The thermostat is working with a sequence represented by a string $s$ consisting of characters 'H' and 'C'.

To maintain 72 degrees, The thermostat must generate a **temp regulation** $t$. A temp regulation is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'H', then $t_i$ must be 'C'.
- If $s_i$ is 'C', then $t_i$ must be 'H'.

The temp regulation $t$ is constructed by reusing the elements available in the original sequence $s$. The thermostat can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 cycle.

Your goal is to construct the longest possible valid temp regulation $t$ (starting from the beginning) using the available counts of 'H's and 'C's from $s$. Calculate the minimum cycles required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
H

#### Output
1

#### Explanation
We have one 'H'. We need a 'C' to oppose $s[0]$. We have no 'C's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
HCC

#### Output
1

#### Explanation
Counts: 'H': 1, 'C': 2.
- Index 0 ($s[0]$='H'): Need 'C'. We have two 'C's. Use one. Remaining: 'H':1, 'C':1.
- Index 1 ($s[1]$='C'): Need 'H'. We have one 'H'. Use one. Remaining: 'H':0, 'C':1.
- Index 2 ($s[2]$='C'): Need 'H'. We have zero 'H's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'H' and 'C'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

