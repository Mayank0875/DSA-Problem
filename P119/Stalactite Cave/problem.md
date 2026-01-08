## Title
Stalactite Cave

## Slug
stalactite-cave

## Difficulty
Medium

## Description
A bat flies through formations. 'V' is a stalactite down, '^' is a stalagmite up.

The structure is represented by a **balanced** parentheses string $s$, where `'V'` signifies diving and `'^'` signifies rising.

The bat wants to find a roost that has a nesting depth of exactly $k$. They can choose to skip certain formations of the structure, effectively using a **subsequence** of the original string. However, the chosen subsequence must still form a valid, balanced sequence.

Your task is to determine if it is possible to select a subsequence of $s$ such that its nesting depth is exactly $k$.

## Examples

### 1

#### Input
2
((()))

#### Output
Yes

#### Explanation
The original depth is 3. We can choose the subsequence corresponding to indices 1, 2, 4, 5 (0-indexed) to get `(())`, which has a nesting depth of 2.

### 2

#### Input
2
()()

#### Output
No

#### Explanation
The maximum nesting depth of the string `()()` is 1. It is impossible to form a depth of 2.

## Input Format
- The first line contains an integer $k$ — the target depth.
- The second line contains a string $s$ of length $n$ consisting of `'V'` and `'^'`.

## Output Format
- Return `Yes` if a subsequence of depth $k$ exists, otherwise output `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ k ≤ n
- The string $s$ is guaranteed to be a balanced parentheses sequence.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string, greedy
