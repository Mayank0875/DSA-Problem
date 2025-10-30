## Title

Busiest T-Shirt Size

## Slug

busiest-t-shirt-size

## Difficulty

Easy

## Description
A marathon organizer is tracking T-shirt size registrations. Sizes are numbered 0 to 100. Given the list of N registered runners and their requested sizes, find the number of shirts needed for the most-requested size. In other words, find the highest frequency among all sizes and print that number.


## Examples

### 1
#### Input
6
10 20 20 30 30 30

#### Output
3

#### Explanation
The maximum frequency is 3 (for mark 30).

### 2
#### Input
7
50 50 40 40 40 50 60

#### Output
3

#### Explanation
Both 40 and 50 appear 3 times; the maximum frequency is 3.

## Input Format
- First line: integer n — number of students.
- Second line: n space-separated integers, each in [0, 100].

## Output Format
- Return a single integer — the maximum frequency among marks.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ mark ≤ 100

## Time Limit
1 second

## Memory Limit
256 MB

## Tags 
counting, array