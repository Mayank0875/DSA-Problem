## Title
Chain Link Assembly

## Slug
chain-link-assembly

## Difficulty
Medium

## Description
A blacksmith forges links. The chain is 'unbroken' from the anchor if links 1 to k are all forged.

There is a sequence of $n$ links indexed from $1$ to $n$. Initially, all links are **missing**.

You forge the links one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you forge the link at the position `sequence[i-1]`.

A state is called **unbroken** if, after performing $k$ steps, exactly the first $k$ links (indices $1$ to $k$) are forged and all other links are missing.

Your task is to calculate how many times the system becomes **unbroken** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "  8  " (Not unbroken)
- Step 2 (index 2): " 88  " (Not unbroken)
- Step 3 (index 4): " 888 " (Not unbroken)
- Step 4 (index 1): "8888 " (unbroken: first 4 are forged)
- Step 5 (index 5): "88888" (unbroken: first 5 are forged)
Total unbroken states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "   8" (Not unbroken)
- Step 2 (index 1): "8  8" (Not unbroken)
- Step 3 (index 2): "88 8" (Not unbroken)
- Step 4 (index 3): "8888" (unbroken)
Total unbroken states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was unbroken.

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
