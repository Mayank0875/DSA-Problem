## Title
Launch Abort

## Slug
launch-abort

## Difficulty
Easy

## Description
A rocket launch countdown (T-minus 10...) is paused. To reset the clock safely, the sequence must be reversed back to the start state.

The data is stored as a string `s`. To reset the countdown, you must reverse the string.

Your challenge is to reverse the string `in-place`, meaning you must modify the given string (or character array) directly. You are not allowed to use extra space for another array. Your solution must use only `O(1)` (constant) extra memory.

## Examples

### 1

#### Input
hello

#### Output
olleh

#### Explanation
The input string `hello` is modified in-place to become `olleh`.

### 2

#### Input
level

#### Output
level

#### Explanation
The input string `level` is modified in-place to become `level`.

## Input Format
- The only input line has a string `s`.

## Output Format
- Return the reversed string without using extra space.

## Constraints
- 3 ≤ s.length ≤ 2000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, two-pointers, in-place
