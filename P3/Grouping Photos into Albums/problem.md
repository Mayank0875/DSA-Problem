## Title

Grouping Photos into Albums

## Slug

grouping-photos-albums

## Difficulty

Easy

## Description

You are organizing digital photos into online albums. Each album page can display either one or two photos. To maintain visual balance, the total 'aesthetic score' (a numerical value assigned to each photo) on a single page cannot exceed a limit `x`. Given the aesthetic scores of `n` photos, determine the minimum number of album pages needed to display all photos according to this rule.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One minimal page arrangement:
    - Page 1: Photo with score 2 and photo with score 7 (Total score 9 <= 10)
    - Page 2: Photo with score 3 (Total score 3 <= 10)
    - Page 3: Photo with score 9 (Total score 9 <= 10)
This requires 3 pages.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One minimal page arrangement:
    - Page 1: Photo with score 2 and photo with score 3 (Total score 5 <= 5)
    - Page 2: Two photos with score 2 (Total score 4 <= 5)
    - Page 3: Photo with score 4 (Total score 4 <= 5)
This requires 3 pages.

## Input Format

- The first line contains two integers n and x: the number of photos and the maximum combined aesthetic score per page.
- The second line contains n integers p_1, p_2, ..., p_n: the aesthetic score of each photo.

## Output Format

- Return a single integer: the minimum number of album pages required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers