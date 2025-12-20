## Title
Library Book Sorting

## Slug
library-book-sorting

## Difficulty
Hard

## Description
Books are shelved by ID. The librarian dislikes it when adjacent books have ID digits that repeat, as it hurts their eyes.

For example, the book ID `12321` is valid because no two adjacent digits are the same. However, `1223` is invalid because the digit `2` appears twice consecutively.

You are given a range of book IDs from $a$ to $b$ (inclusive). Your task is to calculate exactly how many book IDs in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid book IDs between 123 and 321 (inclusive).

### 2

#### Input
1234 1234

#### Output
1

#### Explanation
The number 1234 is valid.

## Input Format
- The input contains two space-separated integers, $a$ and $b$.

## Output Format
- Return a single integer representing the count of valid book IDs in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
