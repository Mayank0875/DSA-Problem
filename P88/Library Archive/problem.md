## Title
Library Archive

## Slug
library-archive

## Difficulty
Medium

## Description
Books have different historical values. To create a 'Master Collection', a selection of books must represent more than half the total value of the library.

Your task is to count the number of **collectionss**. A collection is considered valid if it satisfies two specific criteria:
1.  **Master Status:** The total value of the collection is strictly greater than half of the total value across all books.
2.  **No Superfluous books:** The collection is minimal. This means that removing **any one** book from the collection would cause the remaining total to drop to half or less of the total value (losing the Master Status).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total value is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total value = 10. Half = 5.
Valid collectionss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of books.
- The second line contains n integers: the value of each book.

## Output Format
- Return one integer: the total number of valid collectionss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
