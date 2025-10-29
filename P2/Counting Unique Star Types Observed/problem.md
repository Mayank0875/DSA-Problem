## Title

Counting Unique Star Types Observed

## Slug

counting-unique-star-types-observed

## Difficulty

Easy

## Description

An astronomer is cataloging stars based on their spectral type, represented by a numerical code. Their observation data contains a list of spectral type codes for many observed stars. Some stars of the same type might have been observed and recorded multiple times. The astronomer wants to know the total number of distinct spectral types present in their dataset. Given the list of recorded spectral type codes, calculate the count of unique star types.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The spectral codes recorded are 2, 3, 2, 2, 3. The unique codes are 2 and 3. There are 2 distinct star types in the data.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique codes are 10, 5, and 2. There are 3 distinct star types in the data.

## Input Format

- The first line contains an integer n: the total number of star observations recorded.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the spectral type codes.

## Output Format

- Return a single integer: the count of distinct spectral type codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, astronomy