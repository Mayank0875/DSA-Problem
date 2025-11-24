## Title
Library Shelf Organization

## Slug
library-shelf-organization

## Difficulty
Easy

## Description
A librarian categorizes books into 5 genres: Art, Bio, Cooking, Drama, and Eco. These genres have a strict shelving order (A < B < C < D < E). You need to arrange $n$ books on a shelf such that their genres appear in non-decreasing alphabetical order. How many different genre arrangements are possible for a shelf of $n$ books?

## Examples

### 1

#### Input
1

#### Output
5

#### Explanation
There are 5 valid sequences of length 1.

### 2

#### Input
2

#### Output
15

#### Explanation
There are 15 valid sorted sequences of length 2 (e.g., aa, ae, ai, ao, au, ee, etc.).

## Input Format
- The input consists of a single integer n, representing the required length/quantity.

## Output Format
- Return a single integer representing the total number of valid sorted sequences.

## Constraints
- 1 ≤ n ≤ 50

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math
