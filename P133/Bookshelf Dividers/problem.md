## Title
Bookshelf Dividers

## Slug
bookshelf-dividers

## Difficulty
Medium

## Description
Shelves are filled with books of varying thickness. You want to place a vertical divider that passes between books on as many shelves as possible.

There is a bookcase consisting of $n$ shelves. Each shelf is composed of several books, each having a specific thickness (integers). The total thickness of every shelf is identical.

You need to place a divider from the top to the bottom of the bookcase that minimizes the number of books it hits a book spine on.

If the divider passes exactly through the space between two books, it is **not** considered as hitting a book. However, you cannot place the divider at the very left wall or the very right wall of the bookcase.

Given the 2D array `structure` containing the thicknesss of the books in each shelf, return the minimum number of books hit.

## Examples

### 1

#### Input
6
1 2 2 1
3 1 2
1 3 2
2 4
3 1 2
1 3 1 1

#### Output
2

#### Explanation
The total thickness is 6.
We can place a divider at distance 4 from the left wall.
- Shelf 1: 1+2+2=5 (Hit)
- Shelf 2: 3+1=4 (Space)
- Shelf 3: 1+3=4 (Space)
- Shelf 4: 2 (Hit)
- Shelf 5: 3+1=4 (Space)
- Shelf 6: 1+3=4 (Space)
The divider hits a book spine on shelves 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal spaces. Any divider drawn must hit all 3 books.

## Input Format
- The first line contains an integer $n$, the number of shelves.
- The next $n$ lines each contain space-separated integers representing the thicknesss of the books in that shelf.

## Output Format
- Return a single integer representing the minimum number of books hit.

## Constraints
- 1 ≤ n ≤ 10^4
- 1 <= structure[i].length <= 10^4
- The sum of elements in each row is the same.
- 1 <= structure[i][j] <= 2^31 - 1

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, prefix-sum

