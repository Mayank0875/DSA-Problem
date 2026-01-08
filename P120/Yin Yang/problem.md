## Title
Yin Yang

## Slug
yin-yang

## Difficulty
Medium

## Description
A monk arranges stones. Stones represent Yin ('Y') and Yang ('Z').

The monk is working with a sequence represented by a string $s$ consisting of characters 'Y' and 'Z'.

To create harmony, The monk must generate a **taoist circle** $t$. A taoist circle is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'Y', then $t_i$ must be 'Z'.
- If $s_i$ is 'Z', then $t_i$ must be 'Y'.

The taoist circle $t$ is constructed by reusing the elements available in the original sequence $s$. The monk can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 stone.

Your goal is to construct the longest possible valid taoist circle $t$ (starting from the beginning) using the available counts of 'Y's and 'Z's from $s$. Calculate the minimum stones required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
Y

#### Output
1

#### Explanation
We have one 'Y'. We need a 'Z' to oppose $s[0]$. We have no 'Z's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
YZZ

#### Output
1

#### Explanation
Counts: 'Y': 1, 'Z': 2.
- Index 0 ($s[0]$='Y'): Need 'Z'. We have two 'Z's. Use one. Remaining: 'Y':1, 'Z':1.
- Index 1 ($s[1]$='Z'): Need 'Y'. We have one 'Y'. Use one. Remaining: 'Y':0, 'Z':1.
- Index 2 ($s[2]$='Z'): Need 'Y'. We have zero 'Y's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'Y' and 'Z'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

