## Title

The Librarian's Special Arrangement

## Slug

the-librarians-special-arrangement

## Difficulty

Easy

## Description

In the ancient magical library of Alexandria, books are stored on a long, enchanted shelf. Each book has a specific magical power value. The head librarian wants to reorganize the books based on an old ritual to maintain the balance of energy.

The shelf slots are indexed starting from 0. The ritual requires a specific ordering based on the index of the slot:
1. Books placed at **even indices** (0, 2, 4...) must be sorted in **non-decreasing** order of their power values.
2. Books placed at **odd indices** (1, 3, 5...) must be sorted in **non-increasing** order of their power values.

You are given an array representing the current power values of the books on the shelf. Your task is to rearrange them according to the ritual's rules and return the new arrangement.

## Examples

### 1

#### Input

4
4 1 2 3

#### Output

2 3 4 1

#### Explanation

The values at even indices (0 and 2) are initially 4 and 2. Sorted non-decreasingly, they become 2 and 4.
The values at odd indices (1 and 3) are initially 1 and 3. Sorted non-increasingly, they become 3 and 1.
Recombining them at their respective indices gives [2, 3, 4, 1].
    
### 2

#### Input

2
2 1

#### Output

2 1

#### Explanation

There is only one even index (0) with value 2, and one odd index (1) with value 1. No sorting is needed.
  

## Input Format  

- The first line contains an integer $n$, the number of books.
- The second line contains $n$ space-separated integers representing the power values of the books.

## Output Format  

- Return array containing the n integers in their modified order.
  

## Constraints  

- 1 ≤ n ≤ 1e4
- -1e9 ≤ value[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array