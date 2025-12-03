## Title
Library Book Series

## Slug
library-book-series

## Difficulty
Hard

## Description
A library has n books. References connect some into series. A reader wants a reading list of 'Literary Size' (digits 4 and 7).

The librarian can add references. Merging k series requires k - 1 new references.

Your task is to determine the minimum number of extra references the librarian needs to build to create at least one series whose size is a Literary Size. If this goal cannot be achieved, return -1.

## Examples

### 1

#### Input
4 3
1 2
2 3
1 3

#### Output
1

#### Explanation
The optimal way is to connect book 4 with book 3. We can also connect 4 with 1 or 2. This creates a series of size 4 (a Literary Size).

### 2

#### Input
5 4
1 2
3 4
4 5
3 5

#### Output
-1

#### Explanation
There is no way to connect the books to form a series with a size equal to a Literary Size.

## Input Format
- The first line contains two integers n and m: the number of books and the number of existing references.
- The next m lines each contain two integers u and v, representing a reference between book u and book v. Note that u may be equal to v, and there may be multiple references connecting the same pair of books.

## Output Format
- Return a single integer: the minimum number of references to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
