## Title

Unique Website Visitor IDs

## Slug

unique-website-visitor-ids

## Difficulty

Easy

## Description

A web analyst is tracking visitor traffic to a website. Each visitor session is logged with a numerical visitor ID. Over a period, the same visitor might access the site multiple times, resulting in multiple log entries with the same ID. The analyst wants to determine the number of unique individuals who visited the website during this period. You are given the list of visitor IDs from the log. Find the count of distinct visitor IDs.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The visitor IDs logged are 2, 3, 2, 2, 3. The unique IDs are 2 and 3. There were 2 distinct visitors.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique IDs are 10, 5, and 2. There were 3 distinct visitors.

## Input Format

- The first line contains an integer n: the total number of visitor log entries.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the visitor identification codes.

## Output Format

- Return a single integer: the count of distinct visitor IDs.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, web