## Title

Cryptic Noise

## Slug

cryptic-noise

## Difficulty

Medium

## Description

You are a cryptographer who has discovered a secret key string $s$. To transmit this key safely, you must hide it within a larger string of noise, $t$.

Your task is to rearrange the characters of the noise string $t$ to form a new string $t'$. The secret key $s$ must appear as a **subsequence** in $t'$. This means you can delete zero or more characters from $t'$ to obtain $s$.

Among all possible valid rearrangements of $t$ that contain $s$ as a subsequence, you must find the one that is **lexicographically smallest**. If it is impossible to form such a string (for example, if $t$ does not contain enough of certain characters to build $s$), you should report that it is impossible.

## Examples

### 1

#### Input

dcbe
bedbaecfc

#### Output

abcdcbeef

#### Explanation

The string `abcdcbeef` is a rearrangement of `bedbaecfc`. The subsequence `dcbe` is present (indices 2, 4, 5, 7, roughly). This is the lexicographically smallest arrangement possible.
    
### 2

#### Input

babadab
abacabadabacaba

#### Output

aaaaabababccdab

#### Explanation

`aaaaabababccdab` is the smallest rearrangement of `abacabadabacaba` that contains `babadab` as a subsequence.
  

## Input Format  

- The string $s$ (the secret key).
- The string $t$ (the noise).

## Output Format  

- Return the lexicographically smallest string $t'$. If no such string exists, output "Impossible".
  

## Constraints  

- 1 ≤ |s| ≤ 1e5
- 1 ≤ |t| ≤ 1e5
- Both strings consist of lowercase English letters.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

string, greedy, searching, two-pointers