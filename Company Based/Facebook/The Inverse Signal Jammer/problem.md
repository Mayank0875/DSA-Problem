## Title

The Inverse Signal Jammer

## Slug

the-inverse-signal-jammer

## Difficulty

Medium

## Description

Kai is a network security specialist tasked with neutralizing a malicious broadcast. The broadcast is a binary signal represented by a string $s$ consisting of '0's and '1's. To jam the signal effectively, Kai must generate a counter-signal $t$. 

A counter-signal is valid only if every bit $t_i$ is the exact inverse of the original signal's bit $s_i$ at the same position (meaning $t_i \neq s_i$). The counter-signal $t$ is constructed by reusing the bits available in the original signal $s$. Kai can rearrange the bits of $s$ freely to form $t$, but discarding a bit costs 1 energy unit. 

Your goal is to construct the longest possible valid counter-signal $t$ (starting from index 0) using the available counts of '0's and '1's from $s$. Calculate the minimum energy cost required, which equals the number of bits discarded from $s$.

## Examples

### 1

#### Input

0

#### Output

1

#### Explanation

We have one '0'. We need a '1' to invert $s[0]$. We have no '1's. We must stop immediately. The valid prefix length is 0. We discard the 1 character. Cost = 1.
    
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

- The only input line containing the binary string $s$.

## Output Format  

- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints  

- 1 ≤ |s| ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

string, greedy

## Company
facebook