## Title
Staircase Repair

## Slug
staircase-repair

## Difficulty
Medium

## Description
Steps 1 to n are fixed. The stairs are 'climbable' if steps 1 to k are all safe.

There is a sequence of $n$ steps indexed from $1$ to $n$. Initially, all steps are **broken**.

You fix the steps one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you fix the step at the position `sequence[i-1]`.

A state is called **climbable** if, after performing $k$ steps, exactly the first $k$ steps (indices $1$ to $k$) are fixed and all other steps are broken.

Your task is to calculate how many times the system becomes **climbable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "  -  " (Not climbable)
- Step 2 (index 2): " --  " (Not climbable)
- Step 3 (index 4): " --- " (Not climbable)
- Step 4 (index 1): "---- " (climbable: first 4 are fixed)
- Step 5 (index 5): "-----" (climbable: first 5 are fixed)
Total climbable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "   -" (Not climbable)
- Step 2 (index 1): "-  -" (Not climbable)
- Step 3 (index 2): "-- -" (Not climbable)
- Step 4 (index 3): "----" (climbable)
Total climbable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was climbable.

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
