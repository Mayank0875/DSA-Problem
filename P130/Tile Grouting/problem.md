## Title
Tile Grouting

## Slug
tile-grouting

## Difficulty
Medium

## Description
A tiler grouts spaces between tiles. The floor is 'sealed' from the corner if spaces 1 to k are all grouted.

There is a sequence of $n$ spaces indexed from $1$ to $n$. Initially, all spaces are **open**.

You grout the spaces one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you grout the space at the position `sequence[i-1]`.

A state is called **sealed** if, after performing $k$ steps, exactly the first $k$ spaces (indices $1$ to $k$) are grouted and all other spaces are open.

Your task is to calculate how many times the system becomes **sealed** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "__=__" (Not sealed)
- Step 2 (index 2): "_==__" (Not sealed)
- Step 3 (index 4): "_===_" (Not sealed)
- Step 4 (index 1): "====_" (sealed: first 4 are grouted)
- Step 5 (index 5): "=====" (sealed: first 5 are grouted)
Total sealed states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "___=" (Not sealed)
- Step 2 (index 1): "=__=" (Not sealed)
- Step 3 (index 2): "==_=" (Not sealed)
- Step 4 (index 3): "====" (sealed)
Total sealed states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was sealed.

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
