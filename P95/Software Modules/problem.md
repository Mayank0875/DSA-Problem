## Title
Software Modules

## Slug
software-modules

## Difficulty
Hard

## Description
Functions are grouped into files. The primary purpose of a file is the most frequent function type ID it contains.

The Dev has a collection of $n$ functions, where each function is represented by an integer ID.

To refactor the codebase, The Dev must partition these functions into several non-empty files. Every function from the original collection must belong to exactly one file. From each file, a "primary purpose" is extracted. The primary purpose is defined as the **mode** (most frequent element) of the functions in that file. If a file has multiple functions tied for the most frequent appearance, any one of them can be chosen as the primary purpose.

The Dev collects all the extracted primary purposes to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> primary purpose is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> primary purposes 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> primary purposes 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> primary purposes 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of functions.
- The second line contains $n$ space-separated integers representing the function IDs.

## Output Format
- Return a single integer representing the number of different multisets of primary purposes possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
