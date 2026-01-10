## Title
Book Chapter Reading

## Slug
book-chapter-reading

## Difficulty
Medium

## Description
You are reading a book with n chapters. You read chapters in a random order. The storyline is 'coherent' only when you have read every chapter from 1 up to k continuously.

There is a sequence of $n$ chapters indexed from $1$ to $n$. Initially, all chapters are **unread**.

You finish the chapters one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you finish the chapter at the position `sequence[i-1]`.

A state is called **coherent** if, after performing $k$ steps, exactly the first $k$ chapters (indices $1$ to $k$) are read and all other chapters are unread.

Your task is to calculate how many times the system becomes **coherent** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not coherent)
- Step 2 (index 2): "01100" (Not coherent)
- Step 3 (index 4): "01110" (Not coherent)
- Step 4 (index 1): "11110" (coherent: first 4 are read)
- Step 5 (index 5): "11111" (coherent: first 5 are read)
Total coherent states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not coherent)
- Step 2 (index 1): "1001" (Not coherent)
- Step 3 (index 2): "1101" (Not coherent)
- Step 4 (index 3): "1111" (coherent)
Total coherent states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was coherent.

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
