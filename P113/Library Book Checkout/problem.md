## Title
Library Book Checkout

## Slug
library-book-checkout

## Difficulty
Medium

## Description
Students wait to borrow books. The librarian hands out Fiction (0) and Non-Fiction (1) books from a return stack.

There are two types of books: **Fiction** (represented by `0`) and **Non-Fiction** (represented by `1`). Each student has a specific preference and will only accept one type of book.

The books are prepared in a **stack**, meaning only the top book is accessible at any time. The distribution process works as follows:
1. If the student at the front of the queue prefers the book currently on top of the stack, they take it and leave the queue.
2. If they do not like the top book, they move to the very back of the queue to wait for another turn.

This cycle continues until either all students are served, or the student at the front of the queue (and everyone else behind them) refuses the book currently on top of the stack.

Your task is to determine the number of students who are unable to receive a book.

## Examples

### 1

#### Input
4
1 1 0 0
0 1 0 1

#### Output
0

#### Explanation
* Front student (1) dislikes top book (0), goes to back. Queue: `[1, 0, 0, 1]`.
* Front student (1) dislikes top book (0), goes to back. Queue: `[0, 0, 1, 1]`.
* Front student (0) takes top book (0). Queue: `[0, 1, 1]`, Stack top becomes `1`.
* Front student (0) dislikes top book (1), goes to back. Queue: `[1, 1, 0]`.
* Eventually, all students find their preferred match.

### 2

#### Input
6
1 1 1 0 0 1
1 0 0 0 1 1

#### Output
3

#### Explanation
The top book is `1` (Non-Fiction). Three students prefer Fiction (`0`) and three prefer Non-Fiction (`1`). After the Non-Fiction students take their books, the stack has `0` (Fiction) on top, but only students wanting `1` remain. They cycle endlessly. 3 students remain.

## Input Format
- First line: An integer `n`, the number of students (and books).
- Second line: `n` space-separated integers representing the `preferences` queue.
- Third line: `n` space-separated integers representing the `stack` of books.

## Output Format
- Return a single integer representing the number of students who cannot get a book.

## Constraints
- 1 ≤ n ≤ 100
- `preferences[i]` is `0` or `1`.
- `stack[i]` is `0` or `1`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, queue, array
