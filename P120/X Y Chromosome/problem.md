## Title
X Y Chromosome

## Slug
x-y-chromosome

## Difficulty
Medium

## Description
A geneticist sorts chromosomes. Samples are X ('X') or Y ('Y').

The geneticist is working with a sequence represented by a string $s$ consisting of characters 'X' and 'Y'.

To pair them up, The geneticist must generate a **karyotype** $t$. A karyotype is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'X', then $t_i$ must be 'Y'.
- If $s_i$ is 'Y', then $t_i$ must be 'X'.

The karyotype $t$ is constructed by reusing the elements available in the original sequence $s$. The geneticist can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 chromosome.

Your goal is to construct the longest possible valid karyotype $t$ (starting from the beginning) using the available counts of 'X's and 'Y's from $s$. Calculate the minimum chromosomes required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
X

#### Output
1

#### Explanation
We have one 'X'. We need a 'Y' to oppose $s[0]$. We have no 'Y's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
XYY

#### Output
1

#### Explanation
Counts: 'X': 1, 'Y': 2.
- Index 0 ($s[0]$='X'): Need 'Y'. We have two 'Y's. Use one. Remaining: 'X':1, 'Y':1.
- Index 1 ($s[1]$='Y'): Need 'X'. We have one 'X'. Use one. Remaining: 'X':0, 'Y':1.
- Index 2 ($s[2]$='Y'): Need 'X'. We have zero 'X's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'X' and 'Y'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

