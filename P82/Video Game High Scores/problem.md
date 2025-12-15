## Title
Video Game High Scores

## Slug
video-game-high-scores

## Difficulty
Easy

## Description
A gamer plays n matches. They want to compile a highlight reel showing their skill improvement. The reel should only include matches where the score is strictly better than the previous clip.

You have a list of scores from n matches.
A highlight reel consists of match scores where each score is strictly higher than the preceding one in the reel.

You must edit the clips to find the longest possible improvement streak. You can skip any number of scores to form the sequence, but you must maintain the original chronological order of the selected scores. Calculate the maximum number of scores that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest improvement streaks (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 score.

## Input Format
- The first line contains an integer n: the number of scores.
- The second line contains n integers x_1, x_2 ... x_n: the score of each score in order.

## Output Format
- Return one integer: the length of the longest valid improvement streak.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
