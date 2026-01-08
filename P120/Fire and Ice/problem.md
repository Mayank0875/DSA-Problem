## Title
Fire and Ice

## Slug
fire-and-ice

## Difficulty
Medium

## Description
A mage casts a spell. The elemental stream contains Fire ('F') and Ice ('I') runes.

The mage is working with a sequence represented by a string $s$ consisting of characters 'F' and 'I'.

To stabilize the magic, The mage must generate a **equilibrium spell** $t$. A equilibrium spell is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'F', then $t_i$ must be 'I'.
- If $s_i$ is 'I', then $t_i$ must be 'F'.

The equilibrium spell $t$ is constructed by reusing the elements available in the original sequence $s$. The mage can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 mana point.

Your goal is to construct the longest possible valid equilibrium spell $t$ (starting from the beginning) using the available counts of 'F's and 'I's from $s$. Calculate the minimum mana points required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
F

#### Output
1

#### Explanation
We have one 'F'. We need a 'I' to oppose $s[0]$. We have no 'I's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
FII

#### Output
1

#### Explanation
Counts: 'F': 1, 'I': 2.
- Index 0 ($s[0]$='F'): Need 'I'. We have two 'I's. Use one. Remaining: 'F':1, 'I':1.
- Index 1 ($s[1]$='I'): Need 'F'. We have one 'F'. Use one. Remaining: 'F':0, 'I':1.
- Index 2 ($s[2]$='I'): Need 'F'. We have zero 'F's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'F' and 'I'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

