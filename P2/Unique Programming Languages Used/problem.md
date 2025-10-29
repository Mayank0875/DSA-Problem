## Title

Unique Programming Languages Used

## Slug

unique-programming-languages-used

## Difficulty

Easy

## Description

A software development team tracks the primary programming language used for each project they complete. Each language is represented by a numerical identifier. Over several years, many projects might use the same language. The team lead wants to know the diversity of languages employed by the team, specifically how many different programming languages have been used across all projects. You are given the list of language IDs for all completed projects. Find the count of unique language IDs.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The language IDs are 2, 3, 2, 2, 3. The unique IDs are 2 and 3. The team used 2 distinct programming languages.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique IDs are 10, 5, and 2. The team used 3 distinct programming languages.

## Input Format

- The first line contains an integer n: the total number of projects logged.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the programming language identification codes.

## Output Format

- Return a single integer: the count of distinct language codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, programming