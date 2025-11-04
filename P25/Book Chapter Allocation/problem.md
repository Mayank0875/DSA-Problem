## Title

Book Chapter Allocation

## Slug

book-chapter-allocation

## Difficulty

Medium

## Description

A publisher is editing a book with `n` chapters, arranged in order. Each chapter `i` has `x[i]` pages. The book must be split among `k` editors. Each editor must take a contiguous block of chapters (e.g., editor 1 gets chapters 1-2, editor 2 gets 3-5, etc.). To ensure a balanced workload, the publisher wants to minimize the maximum number of pages any single editor is assigned. Find this minimum value.

## Examples

### 1

#### Input

5 3 
2 4 7 3 5


#### Output

8

#### Explanation

An optimal distribution assigns scrolls [2, 4] to the first scribe (sum 6 pages), scroll [7] to the second scribe (sum 7 pages), and scrolls [3, 5] to the third scribe (sum 8 pages). The maximum number of pages assigned to any scribe is 8. No other distribution into 3 contiguous blocks can achieve a maximum load less than 8.

### 2

#### Input

1 1
34

#### Output

34


#### Explanation

No other distribution into 1 contiguous blocks can achieve a maximum load less than 34.

## Input Format

- The first line contains two integers `n` and `k`: the number of chapters and the number of editors.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the page count of the i-th chapter.

## Output Format

- Return one integer: the minimum possible value for the maximum number of pages assigned to any scribe.

## Constraints

- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ x[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, greedy