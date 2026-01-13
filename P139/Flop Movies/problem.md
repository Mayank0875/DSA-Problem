## Title
Flop Movies

## Slug
flop-movies

## Difficulty
Medium

## Description
A studio reviews film performance.

You have a list of $n$ movies. Each movie has two main properties: **box office revenue** and **critic score**. You are given a 2D integer array `properties` where `properties[i] = [box office revenue_i, critic score_i]` represents the attributes of the $i$-th movie.

A movie is considered **a flop** if there exists another movie that has **both** strictly greater box office revenue and strictly greater critic score.

More formally, the $i$-th movie is a flop if there exists an index $j$ such that `box office revenue_j > box office revenue_i` and `critic score_j > critic score_i`.

Your task is to return the number of a flop movies.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No movie has strictly greater box office revenue and critic score than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first movie (2, 2) is a flop because the second movie (3, 3) has strictly greater box office revenue and critic score.

## Input Format
- The first line contains an integer $n$, the number of movies.
- The next $n$ lines each contain two space-separated integers, representing the box office revenue and critic score of a movie.

## Output Format
- Return a single integer representing the number of a flop movies.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ box office revenue, critic score ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
