## Title
Social Media Likes

## Slug
social-media-likes

## Difficulty
Easy

## Description
An influencer checks likes on n posts. They want to showcase a trend of growing popularity.

You have like counts for n posts.
A popularity trend consists of posts where the like count is strictly higher than the previous selected post.

You must select posts to find the longest possible popularity trend. You can skip any number of posts to form the sequence, but you must maintain the original timeline order of the selected posts. Calculate the maximum number of posts that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest popularity trends (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 post.

## Input Format
- The first line contains an integer n: the number of posts.
- The second line contains n integers x_1, x_2 ... x_n: the like count of each post in order.

## Output Format
- Return one integer: the length of the longest valid popularity trend.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
