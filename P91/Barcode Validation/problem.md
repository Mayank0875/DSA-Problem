## Title
Barcode Validation

## Slug
barcode-validation

## Difficulty
Hard

## Description
A supermarket scanner fails to read barcodes if two adjacent bars have the exact same width ID. Valid barcodes avoid consecutive identical digits.

For example, the barcode `12321` is valid because no two adjacent IDs are the same. However, `1223` is invalid because the ID `2` appears twice consecutively.

You are given a range of barcodes from $a$ to $b$ (inclusive). Your task is to calculate exactly how many barcodes in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid barcodes between 123 and 321 (inclusive).

### 2

#### Input
1234 1234

#### Output
1

#### Explanation
The number 1234 is valid.

## Input Format
- The input contains two space-separated integers, $a$ and $b$.

## Output Format
- Return a single integer representing the count of valid barcodes in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
