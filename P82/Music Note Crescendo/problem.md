## Title
Music Note Crescendo

## Slug
music-note-crescendo

## Difficulty
Easy

## Description
A composer looks at a melody of n notes. They want to extract the longest underlying crescendo, where pitches strictly rise.

You have the pitch values of n notes.
A crescendo consists of notes where each pitch is strictly higher than the previous one.

You must extract notes to find the longest possible crescendo. You can skip any number of notes to form the sequence, but you must maintain the original musical order of the selected notes. Calculate the maximum number of notes that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest crescendos (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 note.

## Input Format
- The first line contains an integer n: the number of notes.
- The second line contains n integers x_1, x_2 ... x_n: the pitch of each note in order.

## Output Format
- Return one integer: the length of the longest valid crescendo.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
