## Title
Musical Melody

## Slug
musical-melody

## Difficulty
Medium

## Description
A composer has selected a set of notes to use in a measure but hasn't decided on the rhythm or order.

The set of notes is represented as a string $S$.
However, the order of the notes is not fixed. Different orderings of the same notes create different melodies.

Your task is to calculate the **total number of distinct melodies** that can be formed using the characters of the string $S$. Since the number of possibilities can be very large, print the result modulo $10^9 + 7$.

## Examples

### 1

#### Input
aabac

#### Output
20

#### Explanation
The string has length 5 with characters {a: 3, b: 1, c: 1}.
Total distinct permutations = $5! / (3! \times 1! \times 1!) = 120 / 6 = 20$.

### 2

#### Input
abc

#### Output
6

#### Explanation
The characters are distinct. The permutations are: "abc", "acb", "bac", "bca", "cab", "cba". Total is 6.

## Input Format
- The first and only line of input contains a string $S$ consisting of lowercase English letters (a–z).

## Output Format
- Return one integer: the number of distinct strings that can be created modulo $10^9+7$.

## Constraints
- 1 ≤ S.length ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
combinatorics, maths, string, hash-table
