## Title
Win Loss Record

## Slug
win-loss-record

## Difficulty
Medium

## Description
A gambler tracks streaks. Results are Win ('W') or Loss ('L').

The gambler is working with a sequence represented by a string $s$ consisting of characters 'W' and 'L'.

To hedge bets, The gambler must generate a **break-even strategy** $t$. A break-even strategy is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'W', then $t_i$ must be 'L'.
- If $s_i$ is 'L', then $t_i$ must be 'W'.

The break-even strategy $t$ is constructed by reusing the elements available in the original sequence $s$. The gambler can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 bet.

Your goal is to construct the longest possible valid break-even strategy $t$ (starting from the beginning) using the available counts of 'W's and 'L's from $s$. Calculate the minimum bets required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
W

#### Output
1

#### Explanation
We have one 'W'. We need a 'L' to oppose $s[0]$. We have no 'L's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
WLL

#### Output
1

#### Explanation
Counts: 'W': 1, 'L': 2.
- Index 0 ($s[0]$='W'): Need 'L'. We have two 'L's. Use one. Remaining: 'W':1, 'L':1.
- Index 1 ($s[1]$='L'): Need 'W'. We have one 'W'. Use one. Remaining: 'W':0, 'L':1.
- Index 2 ($s[2]$='L'): Need 'W'. We have zero 'W's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'W' and 'L'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

