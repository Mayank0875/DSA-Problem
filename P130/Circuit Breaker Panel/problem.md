## Title
Circuit Breaker Panel

## Slug
circuit-breaker-panel

## Difficulty
Medium

## Description
Breakers are flipped on. The house power is 'fully restored' to zone k if breakers 1 to k are on.

There is a sequence of $n$ breakers indexed from $1$ to $n$. Initially, all breakers are **tripped**.

You flip the breakers one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you flip the breaker at the position `sequence[i-1]`.

A state is called **restored** if, after performing $k$ steps, exactly the first $k$ breakers (indices $1$ to $k$) are on and all other breakers are tripped.

Your task is to calculate how many times the system becomes **restored** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not restored)
- Step 2 (index 2): "01100" (Not restored)
- Step 3 (index 4): "01110" (Not restored)
- Step 4 (index 1): "11110" (restored: first 4 are on)
- Step 5 (index 5): "11111" (restored: first 5 are on)
Total restored states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not restored)
- Step 2 (index 1): "1001" (Not restored)
- Step 3 (index 2): "1101" (Not restored)
- Step 4 (index 3): "1111" (restored)
Total restored states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was restored.

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
