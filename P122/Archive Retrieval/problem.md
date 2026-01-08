## Title
Archive Retrieval

## Slug
archive-retrieval

## Difficulty
Hard

## Description
A librarian retrieves files. They grab 1 file or a bound pair of files.

The librarian starts at file 0 and wishes to reach file $n$. On each move, The librarian can pull forward either **1 file** or **2 files**.

Your task is to calculate the total number of distinct ways to reach exactly file $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach file 2:
1. 1 file + 1 file
2. 2 files

### 2

#### Input
3

#### Output
3

#### Explanation
There are three ways:
1. 1 + 1 + 1
2. 1 + 2
3. 2 + 1

## Input Format
- The only input line has an integer $n$ — the target file.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

