## Title
Chemical Sample Analysis

## Slug
chemical-sample-analysis

## Difficulty
Easy

## Description
A lab robot processes vials. Each vial has a unique barcode. Duplicate barcodes in a batch run will crash the machine.

Your task is to determine if any barcode ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The barcode ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All barcode IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of vials.
- The second line contains n space-separated integers, representing the barcode IDs.

## Output Format
- Return `Yes` if any barcode ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
