## Title
Good Evil Karma

## Slug
good-evil-karma

## Difficulty
Medium

## Description
A spirit guide balances souls. Souls have Good ('G') or Evil ('E') karma.

The guide is working with a sequence represented by a string $s$ consisting of characters 'G' and 'E'.

To restore karmic balance, The guide must generate a **redemption arc** $t$. A redemption arc is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'G', then $t_i$ must be 'E'.
- If $s_i$ is 'E', then $t_i$ must be 'G'.

The redemption arc $t$ is constructed by reusing the elements available in the original sequence $s$. The guide can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 soul.

Your goal is to construct the longest possible valid redemption arc $t$ (starting from the beginning) using the available counts of 'G's and 'E's from $s$. Calculate the minimum souls required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
G

#### Output
1

#### Explanation
We have one 'G'. We need a 'E' to oppose $s[0]$. We have no 'E's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
GEE

#### Output
1

#### Explanation
Counts: 'G': 1, 'E': 2.
- Index 0 ($s[0]$='G'): Need 'E'. We have two 'E's. Use one. Remaining: 'G':1, 'E':1.
- Index 1 ($s[1]$='E'): Need 'G'. We have one 'G'. Use one. Remaining: 'G':0, 'E':1.
- Index 2 ($s[2]$='E'): Need 'G'. We have zero 'G's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'G' and 'E'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

