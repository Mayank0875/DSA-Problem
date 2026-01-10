## Title
Solar Panel Array

## Slug
solar-panel-array

## Difficulty
Medium

## Description
Panels in a row come online. The array delivers 'full power' to a sector if panels 1 to k are all active.

There is a sequence of $n$ panels indexed from $1$ to $n$. Initially, all panels are **off**.

You activate the panels one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you activate the panel at the position `sequence[i-1]`.

A state is called **powered** if, after performing $k$ steps, exactly the first $k$ panels (indices $1$ to $k$) are on and all other panels are off.

Your task is to calculate how many times the system becomes **powered** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not powered)
- Step 2 (index 2): "01100" (Not powered)
- Step 3 (index 4): "01110" (Not powered)
- Step 4 (index 1): "11110" (powered: first 4 are on)
- Step 5 (index 5): "11111" (powered: first 5 are on)
Total powered states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not powered)
- Step 2 (index 1): "1001" (Not powered)
- Step 3 (index 2): "1101" (Not powered)
- Step 4 (index 3): "1111" (powered)
Total powered states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was powered.

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
