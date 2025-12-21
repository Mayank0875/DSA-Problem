## Title
Library Sorting

## Slug
library-sorting

## Difficulty
Hard

## Description
Books are bundled for transfer. The category of a bundle is the most frequent genre ID among the books inside.

The Librarian has a collection of $n$ books, where each book is represented by an integer ID.

To organize the archives, The Librarian must partition these books into several non-empty bundles. Every book from the original collection must belong to exactly one bundle. From each bundle, a "category label" is extracted. The category label is defined as the **mode** (most frequent element) of the books in that bundle. If a bundle has multiple books tied for the most frequent appearance, any one of them can be chosen as the category label.

The Librarian collects all the extracted category labels to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> category label is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> category labels 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> category labels 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> category labels 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of books.
- The second line contains $n$ space-separated integers representing the book IDs.

## Output Format
- Return a single integer representing the number of different multisets of category labels possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
