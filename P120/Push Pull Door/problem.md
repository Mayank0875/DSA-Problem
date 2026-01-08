## Title
Push Pull Door

## Slug
push-pull-door

## Difficulty
Medium

## Description
A mechanic fixes automatic doors. The hydraulic commands are Push ('P') or Pull ('U').

The mechanic is working with a sequence represented by a string $s$ consisting of characters 'P' and 'U'.

To calibrate the hinge, The mechanic must generate a **calibration sequence** $t$. A calibration sequence is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'P', then $t_i$ must be 'U'.
- If $s_i$ is 'U', then $t_i$ must be 'P'.

The calibration sequence $t$ is constructed by reusing the elements available in the original sequence $s$. The mechanic can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 command.

Your goal is to construct the longest possible valid calibration sequence $t$ (starting from the beginning) using the available counts of 'P's and 'U's from $s$. Calculate the minimum commands required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
P

#### Output
1

#### Explanation
We have one 'P'. We need a 'U' to oppose $s[0]$. We have no 'U's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
PUU

#### Output
1

#### Explanation
Counts: 'P': 1, 'U': 2.
- Index 0 ($s[0]$='P'): Need 'U'. We have two 'U's. Use one. Remaining: 'P':1, 'U':1.
- Index 1 ($s[1]$='U'): Need 'P'. We have one 'P'. Use one. Remaining: 'P':0, 'U':1.
- Index 2 ($s[2]$='U'): Need 'P'. We have zero 'P's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'P' and 'U'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

