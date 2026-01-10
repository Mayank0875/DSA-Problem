## Title
Puzzle Assembly

## Slug
puzzle-assembly

## Difficulty
Medium

## Description
You are fitting puzzle pieces in a row. The puzzle is 'flush-left' if all pieces from slot 1 to k are filled.

There is a sequence of $n$ pieces indexed from $1$ to $n$. Initially, all pieces are **empty**.

You place the pieces one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you place the piece at the position `sequence[i-1]`.

A state is called **flush-left** if, after performing $k$ steps, exactly the first $k$ pieces (indices $1$ to $k$) are filled and all other pieces are empty.

Your task is to calculate how many times the system becomes **flush-left** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "..X.." (Not flush-left)
- Step 2 (index 2): ".XX.." (Not flush-left)
- Step 3 (index 4): ".XXX." (Not flush-left)
- Step 4 (index 1): "XXXX." (flush-left: first 4 are filled)
- Step 5 (index 5): "XXXXX" (flush-left: first 5 are filled)
Total flush-left states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "...X" (Not flush-left)
- Step 2 (index 1): "X..X" (Not flush-left)
- Step 3 (index 2): "XX.X" (Not flush-left)
- Step 4 (index 3): "XXXX" (flush-left)
Total flush-left states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was flush-left.

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
