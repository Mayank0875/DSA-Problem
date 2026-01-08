## Title
Major Minor Key

## Slug
major-minor-key

## Difficulty
Medium

## Description
A composer writes a symphony. Chords are Major ('M') or Minor ('m').

The composer is working with a sequence represented by a string $s$ consisting of characters 'M' and 'm'.

To evoke emotion, The composer must generate a **chord progression** $t$. A chord progression is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'M', then $t_i$ must be 'm'.
- If $s_i$ is 'm', then $t_i$ must be 'M'.

The chord progression $t$ is constructed by reusing the elements available in the original sequence $s$. The composer can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 chord.

Your goal is to construct the longest possible valid chord progression $t$ (starting from the beginning) using the available counts of 'M's and 'm's from $s$. Calculate the minimum chords required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
M

#### Output
1

#### Explanation
We have one 'M'. We need a 'm' to oppose $s[0]$. We have no 'm's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
Mmm

#### Output
1

#### Explanation
Counts: 'M': 1, 'm': 2.
- Index 0 ($s[0]$='M'): Need 'm'. We have two 'm's. Use one. Remaining: 'M':1, 'm':1.
- Index 1 ($s[1]$='m'): Need 'M'. We have one 'M'. Use one. Remaining: 'M':0, 'm':1.
- Index 2 ($s[2]$='m'): Need 'M'. We have zero 'M's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'M' and 'm'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

