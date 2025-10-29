## Title

Counting Distinct Colors Used

## Slug

counting-distinct-colors-used

## Difficulty

Easy

## Description

An artist is analyzing the palette used for a digital painting. Each color is represented by a unique numerical code (e.g., its RGB value compressed into an integer). The history log shows every color picked by the artist, including repeated selections of the same color. The artist wants to know how many distinct colors were utilized in the artwork. You are given the list of color codes from the history log. Determine the number of unique colors used.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The color codes used are 2, 3, 2, 2, 3. The unique codes are 2 and 3. There are 2 distinct colors.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique codes are 10, 5, and 2. There are 3 distinct colors.

## Input Format

- The first line contains an integer n: the total number of color selections logged.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the numerical color codes.

## Output Format

- Return a single integer: the count of distinct color codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, graphics