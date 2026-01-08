## Title
Input Output

## Slug
input-output

## Difficulty
Medium

## Description
A system administrator checks logs. Logs show Input ('I') and Output ('O') operations.

The admin is working with a sequence represented by a string $s$ consisting of characters 'I' and 'O'.

To verify data integrity, The admin must generate a **I/O match** $t$. A I/O match is valid only if every element $t_i$ is the exact opposite of the original sequence's element $s_i$ at the same position.
- If $s_i$ is 'I', then $t_i$ must be 'O'.
- If $s_i$ is 'O', then $t_i$ must be 'I'.

The I/O match $t$ is constructed by reusing the elements available in the original sequence $s$. The admin can rearrange the elements of $s$ freely to form $t$, but discarding an unused element costs 1 log entry.

Your goal is to construct the longest possible valid I/O match $t$ (starting from the beginning) using the available counts of 'I's and 'O's from $s$. Calculate the minimum log entrys required, which equals the number of elements discarded from $s$.

## Examples

### 1

#### Input
I

#### Output
1

#### Explanation
We have one 'I'. We need a 'O' to oppose $s[0]$. We have no 'O's. We must stop immediately. The valid length is 0. We discard the 1 character. Cost = 1.

### 2

#### Input
IOO

#### Output
1

#### Explanation
Counts: 'I': 1, 'O': 2.
- Index 0 ($s[0]$='I'): Need 'O'. We have two 'O's. Use one. Remaining: 'I':1, 'O':1.
- Index 1 ($s[1]$='O'): Need 'I'. We have one 'I'. Use one. Remaining: 'I':0, 'O':1.
- Index 2 ($s[2]$='O'): Need 'I'. We have zero 'I's. Stop.
Length of $t$ is 2. Total length of $s$ is 3. Cost = $3 - 2 = 1$.

## Input Format
- The only input line containing the string $s$.

## Output Format
- Return a single integer representing the minimum cost (number of discarded characters).

## Constraints
- 1 ≤ |s| ≤ 10^5
- $s$ consists only of characters 'I' and 'O'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy

