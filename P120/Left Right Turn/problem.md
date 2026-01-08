## Title
Left Right Turn

## Slug
left-right-turn

## Difficulty
Medium

## Description
A maze navigator plans a route. Turns are Left ('L') or Right ('R').

The navigator is working with a sequence represented by a string $s$ consisting of characters 'L' and 'R'.

To cancel out deviations, The navigator must generate a **straight path correction** $t$. A straight path correction is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'L', then $t_i$ must be 'R'.
- If $s_i$ is 'R', then $t_i$ must be 'L'.

The straight path correction $t$ is constructed by reusing the elements available in the original sequence $s$. The navigator can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 turn.

Your goal is to construct the longest possible valid straight path correction $t$ (starting from the beginning) using the available counts of 'L's and 'R's from $s$. Calculate the minimum turns required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
L

#### Output
1

#### Explanation
We have one 'L'. We need a 'R' to oppose $s[0]$. We have no 'R's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
LRR

#### Output
1

#### Explanation
Counts: 'L': 1, 'R': 2.
- Index 0 ($s[0]$='L'): Need 'R'. We have two 'R's. Use one. Remaining: 'L':1, 'R':1.
- Index 1 ($s[1]$='R'): Need 'L'. We have one 'L'. Use one. Remaining: 'L':0, 'R':1.
- Index 2 ($s[2]$='R'): Need 'L'. We have zero 'L's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'L' and 'R'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

