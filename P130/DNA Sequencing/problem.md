## Title
DNA Sequencing

## Slug
dna-sequencing

## Difficulty
Medium

## Description
Base pairs are identified. The sequence is 'mapped' from the start if pairs 1 to k are all identified.

There is a sequence of $n$ pairs indexed from $1$ to $n$. Initially, all pairs are **unknown**.

You map the pairs one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you map the pair at the position `sequence[i-1]`.

A state is called **mapped** if, after performing $k$ steps, exactly the first $k$ pairs (indices $1$ to $k$) are identified and all other pairs are unknown.

Your task is to calculate how many times the system becomes **mapped** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "??A??" (Not mapped)
- Step 2 (index 2): "?AA??" (Not mapped)
- Step 3 (index 4): "?AAA?" (Not mapped)
- Step 4 (index 1): "AAAA?" (mapped: first 4 are identified)
- Step 5 (index 5): "AAAAA" (mapped: first 5 are identified)
Total mapped states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "???A" (Not mapped)
- Step 2 (index 1): "A??A" (Not mapped)
- Step 3 (index 2): "AA?A" (Not mapped)
- Step 4 (index 3): "AAAA" (mapped)
Total mapped states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was mapped.

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
