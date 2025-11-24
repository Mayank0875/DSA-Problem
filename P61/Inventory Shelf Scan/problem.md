## Title
Inventory Shelf Scan

## Slug
inventory-shelf-scan

## Difficulty
Medium

## Description
A robot scans a shelf of products, reading their category codes as a string. The warehouse manager wants to identify the longest section of the shelf where every product category is different, to analyze stocking variety. Find the length of this unique section.

## Examples

### 1

#### Input
abcabcbb

#### Output
3

#### Explanation
The answer is "abc", with the length of 3.

### 2

#### Input
bbbbb

#### Output
1

#### Explanation
The answer is "b", with the length of 1.

## Input Format
- The input consists of a single line containing the string `s`.

## Output Format
- Return a single integer representing the maximum length of a substring with unique characters.

## Constraints
- 1 ≤ length(s) ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, hash-table, sliding-window
