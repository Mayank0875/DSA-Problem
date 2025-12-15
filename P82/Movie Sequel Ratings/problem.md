## Title
Movie Sequel Ratings

## Slug
movie-sequel-ratings

## Difficulty
Easy

## Description
A franchise has n movies. A critic wants to find a sub-series where each movie was strictly better received than the last.

You have ratings for n movies.
A rising franchise consists of movies where the rating is strictly higher than the previous one.

You must list the movies to find the longest possible rising franchise. You can skip any number of movies to form the sequence, but you must maintain the original release order order of the selected movies. Calculate the maximum number of movies that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest rising franchises (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 movie.

## Input Format
- The first line contains an integer n: the number of movies.
- The second line contains n integers x_1, x_2 ... x_n: the rating of each movie in order.

## Output Format
- Return one integer: the length of the longest valid rising franchise.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
