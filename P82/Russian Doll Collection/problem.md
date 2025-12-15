## Title
Russian Doll Collection

## Slug
russian-doll-collection

## Difficulty
Easy

## Description
A collector sees n dolls on a shelf. They want to buy a set that can nest inside each other. They must pick dolls from left to right, and each doll must be strictly bigger than the last.

You have the sizes of n dolls.
A nesting set consists of dolls where each doll is strictly larger than the previously picked one.

You must buy dolls to find the longest possible nesting set. You can skip any number of dolls to form the sequence, but you must maintain the original shelf order of the selected dolls. Calculate the maximum number of dolls that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest nesting sets (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 doll.

## Input Format
- The first line contains an integer n: the number of dolls.
- The second line contains n integers x_1, x_2 ... x_n: the size of each doll in order.

## Output Format
- Return one integer: the length of the longest valid nesting set.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
