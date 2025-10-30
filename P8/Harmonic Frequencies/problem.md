## Title

Harmonic Frequencies

## Slug

harmonic-frequencies

## Difficulty

Medium

## Description

A band of N musicians is trying to play in harmony. Each musician `i` is playing a note at a frequency of `A[i]`. The band leader decides they can ask exactly one musician to change their frequency to any value between 1 and 10⁹ (inclusive) to improve the overall sound. The "harmony level" is the greatest common divisor (GCD) of all N frequencies. What is the maximum possible harmony level the band can achieve?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If the leader asks the first musician (playing at frequency 7) to play at frequency 4 instead, the frequencies become [4, 6, 8]. The GCD is 2, which is the maximum possible.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

The leader can ask a musician to play the same frequency they are already playing.

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