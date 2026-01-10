## Title
Inventory Stocking

## Slug
inventory-stocking

## Difficulty
Medium

## Description
Items are placed on numbered shelves. The inventory is 'organized' if shelves 1 to k are filled sequentially.

There is a sequence of $n$ shelves indexed from $1$ to $n$. Initially, all shelves are **empty**.

You stock the shelves one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you stock the shelf at the position `sequence[i-1]`.

A state is called **organized** if, after performing $k$ steps, exactly the first $k$ shelves (indices $1$ to $k$) are stocked and all other shelves are empty.

Your task is to calculate how many times the system becomes **organized** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not organized)
- Step 2 (index 2): "01100" (Not organized)
- Step 3 (index 4): "01110" (Not organized)
- Step 4 (index 1): "11110" (organized: first 4 are stocked)
- Step 5 (index 5): "11111" (organized: first 5 are stocked)
Total organized states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not organized)
- Step 2 (index 1): "1001" (Not organized)
- Step 3 (index 2): "1101" (Not organized)
- Step 4 (index 3): "1111" (organized)
Total organized states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was organized.

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
