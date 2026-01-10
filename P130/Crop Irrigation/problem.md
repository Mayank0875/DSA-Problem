## Title
Crop Irrigation

## Slug
crop-irrigation

## Difficulty
Medium

## Description
Sprinklers turn on in zones 1 to n. The field is 'watered' from the source if zones 1 to k are active.

There is a sequence of $n$ zones indexed from $1$ to $n$. Initially, all zones are **dry**.

You water the zones one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you water the zone at the position `sequence[i-1]`.

A state is called **irrigated** if, after performing $k$ steps, exactly the first $k$ zones (indices $1$ to $k$) are wet and all other zones are dry.

Your task is to calculate how many times the system becomes **irrigated** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "ddwdd" (Not irrigated)
- Step 2 (index 2): "dwwdd" (Not irrigated)
- Step 3 (index 4): "dwwwd" (Not irrigated)
- Step 4 (index 1): "wwwwd" (irrigated: first 4 are wet)
- Step 5 (index 5): "wwwww" (irrigated: first 5 are wet)
Total irrigated states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "dddw" (Not irrigated)
- Step 2 (index 1): "wddw" (Not irrigated)
- Step 3 (index 2): "wwdw" (Not irrigated)
- Step 4 (index 3): "wwww" (irrigated)
Total irrigated states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was irrigated.

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
