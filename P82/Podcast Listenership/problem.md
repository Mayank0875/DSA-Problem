## Title
Podcast Listenership

## Slug
podcast-listenership

## Difficulty
Easy

## Description
A host checks downloads for n episodes. They want to highlight a streak of growing audience.

You have download counts for n episodes.
A growth streak consists of episodes where downloads are strictly higher than the previous episode.

You must review analytics to find the longest possible growth streak. You can skip any number of episodes to form the sequence, but you must maintain the original release order order of the selected episodes. Calculate the maximum number of episodes that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest growth streaks (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 episode.

## Input Format
- The first line contains an integer n: the number of episodes.
- The second line contains n integers x_1, x_2 ... x_n: the downloads of each episode in order.

## Output Format
- Return one integer: the length of the longest valid growth streak.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
