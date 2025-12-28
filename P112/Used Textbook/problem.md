## Title
Used Textbook

## Slug
used-textbook

## Difficulty
Easy

## Description
A student tracks the buyback price of a chemistry book. They want to buy it cheap from a senior and sell it to the bookstore later.

You have a list of book value for $n$ consecutive semesters. You want to make one perfect move: buy used on one semester and sell back on a different semester in the future. You cannot sell back before you buy used.

Your goal is to find the **maximum possible cash back** you can earn from this single transaction. If it is impossible to make any cash back (i.e., the book value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
buy used on semester 2 (book value = 1) and sell back on semester 5 (book value = 6). The cash back is $6 - 1 = 5$.
Note that buy useding on semester 1 (book value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The book value never increases, so it is impossible to make a cash back. The maximum cash back is 0.

## Input Format
- The first line contains a single integer `n`, the number of semesters.
- The second line contains `n` space-separated integers representing the book value on each semester.

## Output Format
- Return a single integer representing the maximum cash back. If no cash back can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
