## Title

Distinct Genetic Markers Found

## Slug

distinct-genetic-markers-found

## Difficulty

Easy

## Description

A biologist is analyzing genetic samples. They identify specific genetic markers, each represented by a unique numerical identifier. In a collection of samples, the same marker might be found multiple times. The biologist needs to determine the diversity of markers present, specifically the count of unique marker IDs found across all samples. You are given the list of all identified marker codes. Find the number of distinct genetic markers.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The marker codes found are 2, 3, 2, 2, 3. The unique codes are 2 and 3. There are 2 distinct genetic markers.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique codes are 10, 5, and 2. There are 3 distinct genetic markers.

## Input Format

- The first line contains an integer n: the total number of markers identified.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the genetic marker identification codes.

## Output Format

- Return a single integer: the count of distinct marker codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, biology