## Title
Asset Tagging

## Slug
asset-tagging

## Difficulty
Easy

## Description
IT dept tags laptops. Duplicate asset tag numbers in the inventory system lead to tracking confusion.

Your task is to determine if any tag number appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The tag number `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All tag numbers are distinct.

## Input Format
- The first line contains a single integer n, the number of assets.
- The second line contains n space-separated integers, representing the tag numbers.

## Output Format
- Return `Yes` if any tag number appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
