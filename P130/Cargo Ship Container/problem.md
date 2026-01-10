## Title
Cargo Ship Container

## Slug
cargo-ship-container

## Difficulty
Medium

## Description
Containers are loaded into slots 1 to n. The stack is 'stable' if slots 1 to k are all filled.

There is a sequence of $n$ slots indexed from $1$ to $n$. Initially, all slots are **empty**.

You fill the slots one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you fill the slot at the position `sequence[i-1]`.

A state is called **stable** if, after performing $k$ steps, exactly the first $k$ slots (indices $1$ to $k$) are filled and all other slots are empty.

Your task is to calculate how many times the system becomes **stable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "__[ ]__" (Not stable)
- Step 2 (index 2): "_[ ][ ]__" (Not stable)
- Step 3 (index 4): "_[ ][ ][ ]_" (Not stable)
- Step 4 (index 1): "[ ][ ][ ][ ]_" (stable: first 4 are filled)
- Step 5 (index 5): "[ ][ ][ ][ ][ ]" (stable: first 5 are filled)
Total stable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "___[ ]" (Not stable)
- Step 2 (index 1): "[ ]__[ ]" (Not stable)
- Step 3 (index 2): "[ ][ ]_[ ]" (Not stable)
- Step 4 (index 3): "[ ][ ][ ][ ]" (stable)
Total stable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was stable.

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
