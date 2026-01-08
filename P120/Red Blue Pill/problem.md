## Title
Red Blue Pill

## Slug
red-blue-pill

## Difficulty
Medium

## Description
A pharmacist sorts pills. The prescription requires alternating Red ('R') and Blue ('B') pills to counter side effects.

The pharmacist is working with a sequence represented by a string $s$ consisting of characters 'R' and 'B'.

To fill the prescription, The pharmacist must generate a **counter-dose** $t$. A counter-dose is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'R', then $t_i$ must be 'B'.
- If $s_i$ is 'B', then $t_i$ must be 'R'.

The counter-dose $t$ is constructed by reusing the elements available in the original sequence $s$. The pharmacist can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 pill.

Your goal is to construct the longest possible valid counter-dose $t$ (starting from the beginning) using the available counts of 'R's and 'B's from $s$. Calculate the minimum pills required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
R

#### Output
1

#### Explanation
We have one 'R'. We need a 'B' to oppose $s[0]$. We have no 'B's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
RBB

#### Output
1

#### Explanation
Counts: 'R': 1, 'B': 2.
- Index 0 ($s[0]$='R'): Need 'B'. We have two 'B's. Use one. Remaining: 'R':1, 'B':1.
- Index 1 ($s[1]$='B'): Need 'R'. We have one 'R'. Use one. Remaining: 'R':0, 'B':1.
- Index 2 ($s[2]$='B'): Need 'R'. We have zero 'R's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'R' and 'B'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

