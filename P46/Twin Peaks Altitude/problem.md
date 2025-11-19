## Title
Twin Peaks Altitude

## Slug
twin-peaks-altitude

## Difficulty
Easy

## Description
A geographer is analyzing elevation data points from a mountain range. They are looking for specific altitude values that appear exactly twice in the survey, as these might indicate twin peaks of equal height. Given the list of altitude measurements, return the values that define these twin peaks.

## Examples

### 1

#### Input
8
1 2 2 3 3 3 4 4

#### Output
2 4

#### Explanation
Value 2 appears twice. Value 4 appears twice. Value 3 appears three times (ignored). Value 1 appears once (ignored). The result is 2 and 4, sorted.

### 2

#### Input
5
5 5 5 6 7

#### Output


#### Explanation
Value 5 appears three times. Values 6 and 7 appear once. No value appears exactly twice.

## Input Format
- First line: integer n — number of elements.
- Second line: n space-separated integers.

## Output Format
- Return all integers that appear exactly twice in increasing order, as a list/array. If none, return an empty list/array.

## Constraints
- 1 ≤ n ≤ 10^5
- Values fit in 32-bit signed integer

## Time Limit
1 second

## Memory Limit
256 MB

## Tags
hash-table, sorting
