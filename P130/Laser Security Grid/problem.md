## Title
Laser Security Grid

## Slug
laser-security-grid

## Difficulty
Medium

## Description
Lasers turn on across a hall. The hall is 'impassable' if lasers 1 to k are active.

There is a sequence of $n$ lasers indexed from $1$ to $n$. Initially, all lasers are **off**.

You arm the lasers one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you arm the laser at the position `sequence[i-1]`.

A state is called **impassable** if, after performing $k$ steps, exactly the first $k$ lasers (indices $1$ to $k$) are on and all other lasers are off.

Your task is to calculate how many times the system becomes **impassable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "  |  " (Not impassable)
- Step 2 (index 2): " ||  " (Not impassable)
- Step 3 (index 4): " ||| " (Not impassable)
- Step 4 (index 1): "|||| " (impassable: first 4 are on)
- Step 5 (index 5): "|||||" (impassable: first 5 are on)
Total impassable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "   |" (Not impassable)
- Step 2 (index 1): "|  |" (Not impassable)
- Step 3 (index 2): "|| |" (Not impassable)
- Step 4 (index 3): "||||" (impassable)
Total impassable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was impassable.

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
