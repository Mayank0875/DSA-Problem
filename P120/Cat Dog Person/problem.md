## Title
Cat Dog Person

## Slug
cat-dog-person

## Difficulty
Medium

## Description
A shelter matches pets. Adopters are Cat ('C') or Dog ('D') people.

The volunteer is working with a sequence represented by a string $s$ consisting of characters 'C' and 'D'.

To find homes, The volunteer must generate a **adoption match** $t$. A adoption match is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'C', then $t_i$ must be 'D'.
- If $s_i$ is 'D', then $t_i$ must be 'C'.

The adoption match $t$ is constructed by reusing the elements available in the original sequence $s$. The volunteer can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 person.

Your goal is to construct the longest possible valid adoption match $t$ (starting from the beginning) using the available counts of 'C's and 'D's from $s$. Calculate the minimum persons required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
C

#### Output
1

#### Explanation
We have one 'C'. We need a 'D' to oppose $s[0]$. We have no 'D's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
CDD

#### Output
1

#### Explanation
Counts: 'C': 1, 'D': 2.
- Index 0 ($s[0]$='C'): Need 'D'. We have two 'D's. Use one. Remaining: 'C':1, 'D':1.
- Index 1 ($s[1]$='D'): Need 'C'. We have one 'C'. Use one. Remaining: 'C':0, 'D':1.
- Index 2 ($s[2]$='D'): Need 'C'. We have zero 'C's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'C' and 'D'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

