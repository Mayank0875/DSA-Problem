## Title
Yes No Vote

## Slug
yes-no-vote

## Difficulty
Medium

## Description
A clerk counts ballots. Votes are Yes ('Y') or No ('N').

The clerk is working with a sequence represented by a string $s$ consisting of characters 'Y' and 'N'.

To determine the outcome, The clerk must generate a **paired vote** $t$. A paired vote is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'Y', then $t_i$ must be 'N'.
- If $s_i$ is 'N', then $t_i$ must be 'Y'.

The paired vote $t$ is constructed by reusing the elements available in the original sequence $s$. The clerk can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 ballot.

Your goal is to construct the longest possible valid paired vote $t$ (starting from the beginning) using the available counts of 'Y's and 'N's from $s$. Calculate the minimum ballots required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
Y

#### Output
1

#### Explanation
We have one 'Y'. We need a 'N' to oppose $s[0]$. We have no 'N's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
YNN

#### Output
1

#### Explanation
Counts: 'Y': 1, 'N': 2.
- Index 0 ($s[0]$='Y'): Need 'N'. We have two 'N's. Use one. Remaining: 'Y':1, 'N':1.
- Index 1 ($s[1]$='N'): Need 'Y'. We have one 'Y'. Use one. Remaining: 'Y':0, 'N':1.
- Index 2 ($s[2]$='N'): Need 'Y'. We have zero 'Y's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'Y' and 'N'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

