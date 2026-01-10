## Title
Encryption Key Fragments

## Slug
encryption-key-fragments

## Difficulty
Medium

## Description
Key fragments are decrypted. The key is 'usable' prefix-wise if fragments 1 to k are all decrypted.

There is a sequence of $n$ fragments indexed from $1$ to $n$. Initially, all fragments are **encrypted**.

You decrypt the fragments one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you decrypt the fragment at the position `sequence[i-1]`.

A state is called **usable** if, after performing $k$ steps, exactly the first $k$ fragments (indices $1$ to $k$) are decrypted and all other fragments are encrypted.

Your task is to calculate how many times the system becomes **usable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "xx1xx" (Not usable)
- Step 2 (index 2): "x11xx" (Not usable)
- Step 3 (index 4): "x111x" (Not usable)
- Step 4 (index 1): "1111x" (usable: first 4 are decrypted)
- Step 5 (index 5): "11111" (usable: first 5 are decrypted)
Total usable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "xxx1" (Not usable)
- Step 2 (index 1): "1xx1" (Not usable)
- Step 3 (index 2): "11x1" (Not usable)
- Step 4 (index 3): "1111" (usable)
Total usable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was usable.

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
