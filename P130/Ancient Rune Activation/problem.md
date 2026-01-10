## Title
Ancient Rune Activation

## Slug
ancient-rune-activation

## Difficulty
Medium

## Description
Runes in a temple floor light up. The magic flow is 'active' if runes 1 to k are all lit.

There is a sequence of $n$ runes indexed from $1$ to $n$. Initially, all runes are **dim**.

You ignite the runes one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you ignite the rune at the position `sequence[i-1]`.

A state is called **active** if, after performing $k$ steps, exactly the first $k$ runes (indices $1$ to $k$) are glowing and all other runes are dim.

Your task is to calculate how many times the system becomes **active** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "..*.." (Not active)
- Step 2 (index 2): ".**.." (Not active)
- Step 3 (index 4): ".***." (Not active)
- Step 4 (index 1): "****." (active: first 4 are glowing)
- Step 5 (index 5): "*****" (active: first 5 are glowing)
Total active states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "...*" (Not active)
- Step 2 (index 1): "*..*" (Not active)
- Step 3 (index 2): "**.*" (Not active)
- Step 4 (index 3): "****" (active)
Total active states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was active.

## Constraints
- 1 ≤ n ≤ 10^4
- `sequence` is a permutation of numbers from $1$ to $n$.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy

## Company
google
