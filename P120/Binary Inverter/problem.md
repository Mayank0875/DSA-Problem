## Title
Binary Inverter

## Slug
binary-inverter

## Difficulty
Medium

## Description
A hacker is writing a virus. The code consists of Zeros ('0') and Ones ('1').

The hacker is working with a sequence represented by a string $s$ consisting of characters '0' and '1'.

To corrupt the system, The hacker must generate a **inverted byte stream** $t$. A inverted byte stream is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is '0', then $t_i$ must be '1'.
- If $s_i$ is '1', then $t_i$ must be '0'.

The inverted byte stream $t$ is constructed by reusing the elements available in the original sequence $s$. The hacker can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 bit.

Your goal is to construct the longest possible valid inverted byte stream $t$ (starting from the beginning) using the available counts of '0's and '1's from $s$. Calculate the minimum bits required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
0

#### Output
1

#### Explanation
We have one '0'. We need a '1' to oppose $s[0]$. We have no '1's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
011

#### Output
1

#### Explanation
Counts: '0': 1, '1': 2.
- Index 0 ($s[0]$='0'): Need '1'. We have two '1's. Use one. Remaining: '0':1, '1':1.
- Index 1 ($s[1]$='1'): Need '0'. We have one '0'. Use one. Remaining: '0':0, '1':1.
- Index 2 ($s[2]$='1'): Need '0'. We have zero '0's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters '0' and '1'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

