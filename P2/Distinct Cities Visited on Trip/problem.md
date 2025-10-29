## Title

Distinct Cities Visited on Trip

## Slug

distinct-cities-visited-trip

## Difficulty

Easy

## Description

A traveler is documenting their journey by recording a numerical code for each city they stop in. Their travel log might list the same city code multiple times if they visited it more than once or passed through it. They want to compile a list of unique cities visited during their trip. Given the sequence of city codes from their log, calculate how many different cities they visited at least once.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The city codes logged are 2, 3, 2, 2, 3. The unique city codes are 2 and 3. The traveler visited 2 distinct cities.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique city codes are 10, 5, and 2. The traveler visited 3 distinct cities.

## Input Format

- The first line contains an integer n: the total number of city entries in the log.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the city identification codes.

## Output Format

- Return a single integer: the count of distinct city codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, travel