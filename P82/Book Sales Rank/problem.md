## Title
Book Sales Rank

## Slug
book-sales-rank

## Difficulty
Easy

## Description
An author tracks the rank of their book over n weeks. They want to show a 'rising star' trajectory by picking weeks where the sales rank improved (rank value gets better/higher sales count).

You have sales numbers for n weeks.
A rising trajectory consists of weeks where sales are strictly higher than the previously selected week.

You must select weeks to find the longest possible success story. You can skip any number of weeks to form the sequence, but you must maintain the original chronological order of the selected weeks. Calculate the maximum number of weeks that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest success storys (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 week.

## Input Format
- The first line contains an integer n: the number of weeks.
- The second line contains n integers x_1, x_2 ... x_n: the sales count of each week in order.

## Output Format
- Return one integer: the length of the longest valid success story.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
