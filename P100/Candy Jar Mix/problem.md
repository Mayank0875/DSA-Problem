## Title
Candy Jar Mix

## Slug
candy-jar-mix

## Difficulty
Medium

## Description
Candies are poured into a thin tube. The candies come in various flavors.

The flavor mix is represented as a string $S$.
However, the order of the candies is not fixed. The visual order of flavors in the tube creates a unique gift pattern.

Your task is to calculate the **total number of distinct candy tubes** that can be formed using the characters of the string $S$. Since the number of possibilities can be very large, print the result modulo $10^9 + 7$.

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
