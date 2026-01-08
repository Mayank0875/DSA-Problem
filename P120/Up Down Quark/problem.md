## Title
Up Down Quark

## Slug
up-down-quark

## Difficulty
Medium

## Description
A particle accelerator detects quarks. The stream has Up ('U') and Down ('D') quarks.

The researcher is working with a sequence represented by a string $s$ consisting of characters 'U' and 'D'.

To form stable mesons, The researcher must generate a **meson chain** $t$. A meson chain is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'U', then $t_i$ must be 'D'.
- If $s_i$ is 'D', then $t_i$ must be 'U'.

The meson chain $t$ is constructed by reusing the elements available in the original sequence $s$. The researcher can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 quark.

Your goal is to construct the longest possible valid meson chain $t$ (starting from the beginning) using the available counts of 'U's and 'D's from $s$. Calculate the minimum quarks required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
U

#### Output
1

#### Explanation
We have one 'U'. We need a 'D' to oppose $s[0]$. We have no 'D's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
UDD

#### Output
1

#### Explanation
Counts: 'U': 1, 'D': 2.
- Index 0 ($s[0]$='U'): Need 'D'. We have two 'D's. Use one. Remaining: 'U':1, 'D':1.
- Index 1 ($s[1]$='D'): Need 'U'. We have one 'U'. Use one. Remaining: 'U':0, 'D':1.
- Index 2 ($s[2]$='D'): Need 'U'. We have zero 'U's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'U' and 'D'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

