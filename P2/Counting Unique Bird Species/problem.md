## Title

Counting Unique Bird Species

## Slug

counting-unique-bird-species

## Difficulty

Easy

## Description

A birdwatcher has spent the day documenting the species of birds they observed. Each bird species is identified by a unique numerical code. Throughout the day, they might have seen the same species multiple times. Now, they want to know how many different species of birds they actually spotted. You are given the list of species codes recorded for every bird sighting. Help the birdwatcher determine the count of unique species observed.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The species codes recorded are 2, 3, 2, 2, 3. The unique codes are 2 and 3. There are 2 distinct bird species.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique codes are 10, 5, and 2. There are 3 distinct species types.

## Input Format

- The first line contains an integer n: the total number of bird sightings.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the species identification codes.

## Output Format

- Return a single integer: the count of distinct species codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting