## Title

Code Library Compatibility

## Slug

code-library-compatibility

## Difficulty

Medium

## Description

You are trying to build a project using N different code libraries. Each library `i` has a version number `A[i]`. To avoid conflicts, all N library versions should be multiples of a common "base version" number. You are allowed to replace exactly one library with a different one, which can have any version number from 1 to 10⁹. What is the maximum possible "base version" (GCD) you can achieve for your project?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If you replace version 7 with version 4, the library versions [4, 6, 8] are all compatible with a base version of 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

You can replace a library with another one of the same version.

## Input Format

- First line: integer 'n' representing the number of elements written on the blackboard .  
- Second line: 'n' integers representing the elements that are written on blackboard.
- You will be given the array as an input to your function

## Output Format

- Return an integer representing the greatest common divisor after making your move.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, suffix sum, math