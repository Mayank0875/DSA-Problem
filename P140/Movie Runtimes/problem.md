## Title
Movie Runtimes

## Slug
movie-runtimes

## Difficulty
Easy

## Description
A film festival schedules shorts and features based on duration.

The submission form records the duration (mins) of $N$ movies in an array. To plan the screenings, the scheduler needs to assign a rank to every movie based on its duration (mins).

The ranking rules are simple: the movie with the **smallest** duration (mins) gets **Rank 1**. The next distinct duration (mins) gets **Rank 2**, and so on.

If two or more movies have the exact same duration (mins), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each movie's duration (mins) with its corresponding rank.

## Examples

### 1

#### Input
4
40 10 20 30

#### Output
4 1 2 3

#### Explanation
10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).

### 2

#### Input
3
2 2 2

#### Output
1 1 1

#### Explanation
All movies share the same duration (mins), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of movies.
- The second line contains `n` space-separated integers representing the duration (mins)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding movie.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
