## Title

The Abyssal Layers

## Slug

the-abyssal-layers

## Difficulty

Medium

## Description

A deep-sea diver is exploring a mysterious trench system. The structure of the trench is represented by a **balanced** parentheses string $s$, where `'('` signifies descending into a deeper layer and `')'` signifies ascending back up.

The diver wants to plan a route that reaches a specific nesting depth, $k$. They can choose to skip certain sections of the trench, effectively traveling through a **subsequence** of the original structure. However, the chosen path must still form a valid, balanced parentheses sequence.

Your task is to determine if it is possible to select a subsequence of $s$ such that its nesting depth is exactly $k$.

## Examples

### 1

#### Input

2
((()))

#### Output

true

#### Explanation

The original depth is 3. We can choose the subsequence corresponding to indices 1, 2, 4, 5 (0-indexed) to get `(())`, which has a nesting depth of 2.
    
### 2

#### Input

2
()()

#### Output

false

#### Explanation

The maximum nesting depth of the string `()()` is 1. It is impossible to form a depth of 2.

## Input Format  

- Integers $k$ — the target depth.
- A string $s$ of length $n$ consisting of `'('` and `')'`.

## Output Format  

- Return `true` if a subsequence of depth $k$ exists, otherwise output `false`.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ k ≤ n
- The string $s$ is guaranteed to be a balanced parentheses sequence.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, string, greedy