## Title
Vending Machine Stock

## Slug
vending-machine-stock

## Difficulty
Medium

## Description
Slots are refilled. The row is 'fully stocked' up to slot k if slots 1 to k all have items.

There is a sequence of $n$ slots indexed from $1$ to $n$. Initially, all slots are **empty**.

You refill the slots one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you refill the slot at the position `sequence[i-1]`.

A state is called **stocked** if, after performing $k$ steps, exactly the first $k$ slots (indices $1$ to $k$) are full and all other slots are empty.

Your task is to calculate how many times the system becomes **stocked** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not stocked)
- Step 2 (index 2): "01100" (Not stocked)
- Step 3 (index 4): "01110" (Not stocked)
- Step 4 (index 1): "11110" (stocked: first 4 are full)
- Step 5 (index 5): "11111" (stocked: first 5 are full)
Total stocked states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not stocked)
- Step 2 (index 1): "1001" (Not stocked)
- Step 3 (index 2): "1101" (Not stocked)
- Step 4 (index 3): "1111" (stocked)
Total stocked states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was stocked.

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
