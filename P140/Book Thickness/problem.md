## Title
Book Thickness

## Slug
book-thickness

## Difficulty
Easy

## Description
A librarian arranges books by page count for a special display.

The catalog records the page count of $N$ books in an array. To organize the shelf, the librarian needs to assign a rank to every book based on its page count.

The ranking rules are simple: the book with the **smallest** page count gets **Rank 1**. The next distinct page count gets **Rank 2**, and so on.

If two or more books have the exact same page count, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each book's page count with its corresponding rank.

## Examples

### 1

#### Input
4
40 10 20 30

#### Output
4 1 2 3

#### Explanation
10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).

### 2

#### Input
3
2 2 2

#### Output
1 1 1

#### Explanation
All books share the same page count, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of books.
- The second line contains `n` space-separated integers representing the page counts.

## Output Format
- Return an array of integers where each element is the rank of the corresponding book.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
