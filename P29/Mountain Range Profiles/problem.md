## Title

Mountain Range Profiles

## Slug

mountain-range-profiles

## Difficulty

Easy

## Description

You are a cartographer drawing mountain ranges. You represent a mountain range as a sequence of up-strokes and down-strokes. You are given $n$ up-strokes and $n$ down-strokes. A valid 'mountain range' starts at sea level, never goes below sea level, and ends at sea level. Your task is to determine how many different valid mountain range profiles you can draw using exactly $n$ up-strokes and $n$ down-strokes.
## Examples

### 1

#### Input

3

#### Output

5

#### Explanation

The 5 unique well-formed combinations are:
((()))
(()())
(())()
()(())
()()()

### 2

#### Input

1

#### Output

1

#### Explanation
The only combination is ().

## Input Format  

- The input consists of a single line containing one integer, `n`.

## Output Format  

- Return single integer representing total number of well-formed parenthesis combinations.
  

## Constraints  

- 1 ≤ n ≤ 8

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion