## Title

Code Module Optimization

## Slug

code-module-optimization

## Difficulty

Medium

## Description

A large software project has N modules. The memory footprint of each module `i` is `A[i]` kilobytes. You are an optimizer. You can choose exactly one module to completely refactor. After refactoring, the module can have any memory footprint from 1 to 10⁹ KB. Your goal is to choose the refactor target to maximize the "common memory block" (GCD of all footprints) for the N modules.

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If you refactor the 7KB module to be 4KB, the footprints [4, 6, 8] have a GCD of 2. This is the maximum possible.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

Refactoring a 100KB module to 100KB is a valid (though not very effective) move.

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