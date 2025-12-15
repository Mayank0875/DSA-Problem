## Title
Library Book Repair

## Slug
library-book-repair

## Difficulty
Medium

## Description
A library sends `n` damaged books to `m` binders.

However, not every book is compatible with every binder due to repair type needed.
You are given a list of `k` compatible pairs, where a specific book can work with a specific binder.

Your task is to determine the maximum number of repairs that can be formed simultaneously. Each book and each binder can be assigned to at most one repair.

## Examples

### 1

#### Input
3 2 4
1 1
1 2
2 1
3 1

#### Output
2

#### Explanation
There are 3 books and 2 binders.
Possible valid matching could be:
- book 1 with binder 2
- book 2 with binder 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only book 1 and binder 1 are compatible. The maximum number of operational repairs is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of books, binders, and compatible pairs.
- The books are numbered `1` to `n` and the binders are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that book `a` and binder `b` are compatible.

## Output Format
- Return one integer: the maximum number of pairs that can be formed.

## Constraints
- 1 ≤ n, m ≤ 500
- 1 ≤ k ≤ 1000
- 1 ≤ a ≤ n
- 1 ≤ b ≤ m

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
