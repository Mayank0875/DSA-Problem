## Title
Start Stop Button

## Slug
start-stop-button

## Difficulty
Medium

## Description
A machine operator presses buttons. Commands are Start ('S') or Stop ('X').

The operator is working with a sequence represented by a string $s$ consisting of characters 'S' and 'X'.

To run the cycle, The operator must generate a **control sequence** $t$. A control sequence is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'S', then $t_i$ must be 'X'.
- If $s_i$ is 'X', then $t_i$ must be 'S'.

The control sequence $t$ is constructed by reusing the elements available in the original sequence $s$. The operator can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 press.

Your goal is to construct the longest possible valid control sequence $t$ (starting from the beginning) using the available counts of 'S's and 'X's from $s$. Calculate the minimum presss required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
S

#### Output
1

#### Explanation
We have one 'S'. We need a 'X' to oppose $s[0]$. We have no 'X's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
SXX

#### Output
1

#### Explanation
Counts: 'S': 1, 'X': 2.
- Index 0 ($s[0]$='S'): Need 'X'. We have two 'X's. Use one. Remaining: 'S':1, 'X':1.
- Index 1 ($s[1]$='X'): Need 'S'. We have one 'S'. Use one. Remaining: 'S':0, 'X':1.
- Index 2 ($s[2]$='X'): Need 'S'. We have zero 'S's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'S' and 'X'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

