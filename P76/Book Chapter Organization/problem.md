## Title
Book Chapter Organization

## Slug
book-chapter-organization

## Difficulty
Hard

## Description
An editor is formatting a book with `n` articles into `k` chapters. Each article has a page count. Articles must remain in order. The 'bulkiness' of a chapter is the square of its total page count.

You must partition the sequence of articles into exactly `k` non-empty contiguous chapters.
Each chapter corresponds to a chapter.
The "bulkiness" for a chapter is calculated as the **square of the sum** of the page counts of the articles in that chapter.

Your goal is to minimize the total bulkiness (the sum of the bulkiness values of all `k` chapters).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the articles into 3 chapters: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total bulkiness is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 chapter is allowed, containing all articles. Sum = 15. bulkiness = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of articles and the required number of chapters.
- The second line contains `n` integers representing the page counts of each article.

## Output Format
- Return one integer: the minimum total bulkiness.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
