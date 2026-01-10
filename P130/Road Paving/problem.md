## Title
Road Paving

## Slug
road-paving

## Difficulty
Medium

## Description
A crew paves mile markers. The road is 'drivable' from the start if miles 1 to k are all paved.

There is a sequence of $n$ miles indexed from $1$ to $n$. Initially, all miles are **dirt**.

You pave the miles one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you pave the mile at the position `sequence[i-1]`.

A state is called **drivable** if, after performing $k$ steps, exactly the first $k$ miles (indices $1$ to $k$) are paved and all other miles are dirt.

Your task is to calculate how many times the system becomes **drivable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "~~=~~" (Not drivable)
- Step 2 (index 2): "~==~~" (Not drivable)
- Step 3 (index 4): "~===~" (Not drivable)
- Step 4 (index 1): "====~" (drivable: first 4 are paved)
- Step 5 (index 5): "=====" (drivable: first 5 are paved)
Total drivable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "~~~=" (Not drivable)
- Step 2 (index 1): "=~~=" (Not drivable)
- Step 3 (index 2): "==~=" (Not drivable)
- Step 4 (index 3): "====" (drivable)
Total drivable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was drivable.

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
